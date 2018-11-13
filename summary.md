## StringTest
- should_be_immutable()
1. The knowledge point of this unit test is to know that a string is immutable, the replace() method will return a new string as a result while not affecting the original string. Offical document: https://docs.oracle.com/javase/tutorial/java/data/strings.html, https://docs.oracle.com/javase/tutorial/java/data/manipstrings.html
2. The original expected result is null value at first.
3. Since the replace method return a modified string and assigned to variable "modifiedString" while not affecting the original string, the comparision between these two strings will return false.
4. No

- all_modification_method_will_create_new_string()
1. The knowledge point of this unit test is to know that a string is immutable, the trim() method will return a new string as a result while not affecting the original string. Offical document: https://docs.oracle.com/javase/tutorial/java/data/strings.html, https://docs.oracle.com/javase/tutorial/java/data/manipstrings.html
2. The original expected result is null value at first.
3. Since the trim method return a modified string and assigned to variable "modifiedString" while not affecting the original string, the comparision between these two strings will return false.
4. No

- will_create_new_string_when_concat()
1. The knowledge point of this unit test is to know that a string is immutable, the += opeartion will return a new string as a result while not affecting the original string. Offical document: https://docs.oracle.com/javase/tutorial/java/data/strings.html, https://docs.oracle.com/javase/tutorial/java/data/manipstrings.html
2. The original expected result is null value at first.
3. The value of original string is assigned to the variable "copyOfOriginalString", after that when we use += operation on the variable "originalString", it actuals create a new string and assigns to it. Thus the value of "copyOfOriginalString" isn't changed, so the comparision between these two strings will return false.
4. No

- should_taken_string_apart()
1. The knowledge point of this unit test is to know the Java provided method to get a substring. Offical document: https://docs.oracle.com/javase/tutorial/java/data/manipstrings.html
2. The original expected result is null value at first.
3. Call the substring() method of the origin string, and index = 5 as the wanted string is started from the world "is", without the "Java " at the first of the original string, which index is 0 to 4. Thus substring(5) will return the result wanted.
4. No

- should_taken_string_apart_continued()
1. The knowledge point of this unit test is to know the Java provided method to get a substring. Offical document: https://docs.oracle.com/javase/tutorial/java/data/manipstrings.html
2. The original expected result is null value at first.
3. Call the substring() method of the origin string, since the string "is" is of the index 5 and 6 from the original string. Hence calling the substring(5, 7) will return the string "is". (As the second parameter index is not included in the return string)
    * - What if the input arguments is out of range of the string?
      - It will throw StringIndexOutOfBoundException.
    * - What will happen if the the starting index is greater than the ending index?
      - It will throw StringIndexOutOfBoundException.
    * - What will happen if the input string is of null reference?
      - It will throw NullPointerException.
4. No

- should_break_string_into_words()
1. The knowledge point of this unit test is to know the Java provided method to split a string into string array based on the input delimeter. Offical document: https://docs.oracle.com/javase/tutorial/java/data/manipstrings.html
2. The original expected result is null value at first.
3. Call the split() method on the original string. As the delimeter is a space character, called split(" ") will split the string into each word which is the desired array.
4. No

- should_break_string_into_words_customized()
1. The knowledge point of this unit test is to know the Java provided method to split a string into string array based on the input delimeter. Offical document: https://docs.oracle.com/javase/tutorial/java/data/manipstrings.html
2. The original expected result is null value at first.
3. Call the split() method on the original string. As the delimeter is a slash character, called split("/") will split the string into each word which is the desired array.
4. No

- should_create_ascii_art()
1. The knowledge point of this unit test is to use the StringBuilder class to construct a string. Offical document: https://docs.oracle.com/javase/tutorial/java/data/buffers.html
2. The original expected result is null value at first.
3. Call the append() method of the StringBuilder, and append each string which is appended by += operator for the expected string. And thus they will result in a same value.
4. No

- should_calculate_checksum_of_a_string()
1. The knowledge point of this unit test is to use the provided method to convert a String to a Char array. Offical document: https://docs.oracle.com/javase/tutorial/java/data/strings.html
2. The original expected result is null value at first.
3. Call the toCharArray() method of the original string, for each character, add the value of that character into the sum variable, and the result will be our checksum.
4. No

- should_convert_unicode_escape()
1. The knowledge point of this unit test is to use the provided method to know the escape method for unicode. Offical document: https://docs.oracle.com/javase/specs/jls/se7/html/jls-3.html
2. The original expected result is null value at first.
3. For each unicode character, put a "\u" before its unicode value. So the desire string could be built as "\u306a\u306b\u3053\u308c".
4. No

- should_reverse_a_string()
1. The knowledge point of this unit test is to use the provided method to know reverse method for StringBuilder class. Offical document: https://docs.oracle.com/javase/tutorial/java/data/buffers.html
2. The original expected result is null value at first.
3. Create a StringBuilder Object, call its reverse() method and thus we can get the reversed string as result.
4. No

- should_compare_string_with_different_cases()
1. The knowledge point of this unit test is to know the comparison result of equals() and equalsIgnoreCase(). Offical document: https://docs.oracle.com/javase/tutorial/java/data/comparestrings.html
2. The original expected result is null value at first.
3. As the first comparsion is only calling equals(), the result is false as one string is all capital letter and the other is not. The second comparison is calling equalsIgnoreCase(), so the upper case and lower case will not affect the comparison, so the result is true.
4. No

- should_format_string()
1. The knowledge point of this unit test is to know the result of String.format(). Offical document: https://docs.oracle.com/javase/tutorial/java/data/strings.html
2. The original expected result is null value at first.
3. The expected result should be "Hello, Harry. Next year, you will be 23." as it put the value of name into that %s which put "Harry" there, an put the value of age into that %d which put "23" there. As a result the formatted string is like that.
4. No



