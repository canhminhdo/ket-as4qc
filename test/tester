#!/bin/sh

echo "~~~~~~~~~~ TESTING ~~~~~~~~~~"
DIR="output"
ls | grep ".maude$" | sort -V | while read -r FILE; do
    NAME=`echo $FILE | cut -d '.' -f1`
    maude < $FILE -no-banner | sed -r '/^(rewrites:|states:)/d' > "$DIR/$NAME.out"
    diff "$DIR/$NAME.expected" "$DIR/$NAME.out"
    rm "$DIR/$NAME.out"
done
echo "DONE!"