# 51talk
data analysis

find the length of calls(mins)
for file in *.mp3; do mp3info -p "%S\n" "$file"; done | paste -sd+ | sed 's+\(.*\)+(\1)/60+' | bc

find the length of calls(sec)
for file in *.mp3; do mp3info -p "%S\n" "$file"; done | paste -sd+ | sed 's+\(.*\)+(\1)+' | bc

