# geometry

Constants.IO_DEFAULT - JRecord will decide the actual method based on other values (The Default Value). It is generally better to explicitly set the File-Organisation (or file-Structure).
Constants.IO_STANDARD_TEXT_FILE - Standard Windows/*nix/Mac text file using \n, \n\r etc as a record (or line) delimiter.
Constants.IO_UNICODE_TEXT - Standard Windows/*nix/Mac Unicode / double byte text file using \n, \n\r etc as a record (or line) delimiter. It ensures record are stored in character format (instead of bytes).
Constants.IO_FIXED_LENGTH - Every Record (or line) is a standard Fixed length based on the Maximum schema length.
Constants.IO_FIXED_LENGTH_CHAR - Fixed length character file (typically used for Fixed-Length unicode files).
Constants.IO_VB - Mainframe VB (Variable Record length file). Records consist of a Record-Length followed by the Record-Data.
Constants.IO_VB_DUMP - Raw Block format of a Mainframe-VB file. You get this format if you specify RECFM=U when reading it on the mainframe.
Constants.IO_VB_GNU_COBOL - GNU (open-Cobol) VB format.


Unlike on Linux / Windows most Text files are going to have \n or \r\n marking the End of Line.
On The mainframe the situation is quite different; the 2 main ways for organising lines are
FB - Fixed length records - every record is a constant fixed length; there are no \n (or \r) line markers
VB - Variable Length record - each record starts with a Record Length and is followed the lines text or data. Again there is no \n (or \r) line markers
