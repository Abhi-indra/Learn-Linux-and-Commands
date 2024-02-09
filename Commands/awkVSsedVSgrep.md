# AWK vs SED vs GREP

**AWK**

AWK is a versatile programming language primarily used for text processing and data extraction. It operates on a line-by-line basis and is well-suited for processing structured data. AWK allows users to define patterns and actions to be taken when those patterns are matched.

**Key Features:**
- **Pattern Matching**: AWK scans input lines and matches them against specified patterns.
- **Field Parsing**: It automatically splits input lines into fields based on whitespace or specified delimiters.
- **Built-in Variables**: AWK provides built-in variables like `$0` (entire line), `$1`, `$2`, etc. (individual fields), and `NF` (number of fields).
- **Custom Actions**: Users can define custom actions to be executed when patterns are matched.
- **Text Transformation**: AWK facilitates text transformation by modifying input lines or generating new output based on specified criteria.

**Usage Examples:**
1. Print lines containing a specific pattern:
   ```
   awk '/pattern/' file.txt
   ```

2. Print specific fields from a file:
   ```
   awk '{print $1, $3}' file.txt
   ```

3. Calculate and print the total of a column:
   ```
   awk '{total += $2} END {print "Total:", total}' file.txt
   ```

4. Apply conditional statements for more complex processing:
   ```
   awk '$3 > 50 {print $1, $2}' file.txt
   ```

**SED**

SED (Stream Editor) is a powerful command-line tool for text manipulation. It processes input line by line and applies specified operations, making it useful for tasks like search and replace, text transformation, and file editing.

**Key Features:**
- **Search and Replace**: SED can search for specific patterns in text and replace them with other patterns.
- **Global Operations**: It can apply operations globally across the input text or within specified ranges.
- **Regular Expressions**: SED supports regular expressions for pattern matching and manipulation.
- **In-place Editing**: SED can edit files in-place without requiring temporary files.
- **Multiple Commands**: SED allows chaining multiple commands together for complex text processing tasks.

**Usage Examples:**
1. Search and replace text in a file:
   ```
   sed 's/pattern/replacement/' file.txt
   ```

2. Delete lines matching a specific pattern:
   ```
   sed '/pattern/d' file.txt
   ```

3. Print specific lines or ranges of lines:
   ```
   sed -n '1,5p' file.txt
   ```

4. Perform text substitution globally:
   ```
   sed 's/pattern/replacement/g' file.txt
   ```

**GREP**

GREP is a command-line utility used for searching text files for lines that match a specified pattern. It's a powerful tool for quickly finding information within files and directories.

**Key Features:**
- **Pattern Matching**: GREP searches for specified patterns in text files using regular expressions.
- **Contextual Output**: It can display lines before or after matches, or both, providing context for the matched lines.
- **Recursive Search**: GREP can search recursively through directories and subdirectories.
- **Case Insensitivity**: It supports case-insensitive searches.
- **Output Control**: GREP offers options to control the format and verbosity of the output.

**Usage Examples:**
1. Search for a specific pattern in a file:
   ```
   grep 'pattern' file.txt
   ```

2. Search for a pattern recursively in a directory:
   ```
   grep -r 'pattern' directory/
   ```

3. Display lines containing a pattern, along with line numbers:
   ```
   grep -n 'pattern' file.txt
   ```

4. Perform a case-insensitive search:
   ```
   grep -i 'pattern' file.txt
   ```

**Conclusion:**

AWK, SED, and GREP are powerful tools for text processing and manipulation on the command line. E