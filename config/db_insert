#!/usr/bin/env bash
cut_size="$1"    # e.g. "head -1"
device_size="$2" # e.g. "pc_size"
device_url="$3"  # e.g. "pc_url"

start=$SECONDS

function update_db() {
    mapfile -t website_links < <(sqlite3 mods.db "SELECT website_url FROM mods where pc_size is null or android_size is null;")
    mod_size=()
    local i=0
    for url in "${website_links[@]}"; do
        mod_size+=("$(curl -s "$url" | grep 'Mb]' | cut -d [ -f 2 | cut -d ] -f 1 | cut -d M -f 1 | uniq | $cut_size)")
        sqlite3 mods.db "UPDATE mods SET $device_size = '${mod_size[$i]}' WHERE $device_url IS NOT NULL AND website_url = '$url';"
        ((i++))
    done
    echo "Done in $((SECONDS - start))s"
}

update_db

# ./db_insert.sh "head -1" "android_size" "android_url"
# ./db_insert.sh "tail -1" "pc_size" "pc_url"
