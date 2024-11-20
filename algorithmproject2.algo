ALGORITHM insertion_sort
VAR
    i, j, n, temp : INTEGER
    arr : ARRAY_OF INTEGER[100];  // limit sort size to 100 numbers
BEGIN

    // get how many numbers to be sorted betweeen 1 and 100
    REPEAT
        Write ("How many numbers are to be sorted? (between 1 and 100): ")
        Read (n)
    UNTIL (n > 0 AND n <= 100)

    // get numbers to be sorted
    Write ("Enter numbers to be sorted one after another:")
    FOR i FROM 0 TO n-1 STEP 1  DO
        Read (arr[i])
    END_FOR

    // commence insertion sorting
    // starting from the second item in the array, loop through till the last item
    FOR i FROM 1 TO n - 1 STEP 1  DO
        temp = arr[i]                              // assign the selected ith item to a temporary location
        FOR j FROM i-1 TO 0 STEP step  -1           // starting from the item to the left of the selected ith item loop through till the first item
            IF (temp < arr[j]) THEN                 // check if the ith item put in a temporary storage is smaller than the current jth item
                arr[j+1] = arr[j]                 // if the temp is smaller, move the jth item one step to the right
                arr [j] = temp                     // then move the temp item into the j-th location
            ELSE
                BREAK;                              // If temp is larger than jth item, then break out of inner loop
            END_IF
        END_FOR
    END_FOR
    Write (arr)                                    // Print out sorted array
END