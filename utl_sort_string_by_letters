Sort letters in string alphabetically

HAVE
====

  myword = 'the quick brown fox jumps over the lazy dog';

WANT  (sort the leaders (probably need full SAS (not server EG, UE or SAS Studio?)
====

  MYWORD=abcdeeefghhijklmnoooopqrrsttuuvwxyz

*          _       _   _
 ___  ___ | |_   _| |_(_) ___  _ __
/ __|/ _ \| | | | | __| |/ _ \| '_ \
\__ \ (_) | | |_| | |_| | (_) | | | |
|___/\___/|_|\__,_|\__|_|\___/|_| |_|
;

data _null_;
    myword = 'the quick brown fox jumps over the lazy dog';
    array letters[43] $1 ;
    call pokelong(myword,addrlong(letters1),43); /*Limit # of chars to copy to the length of array*/
    call sortc(of letters[*]);
    myword = cat(of letters[*]);
    putlog myword=;
run;quit;

