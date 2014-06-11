chext
=====

Sometimes I get lots of "*.PNG" files in my directory.  I would prefer the extention to be lowercase:

  $ chext .PNG .png *.PNG

Actually, if the list of files is omitted, the script examines the files in the current directory, so

  $ chext .PNG .png

is equivalent.  Sometimes the extention is just plain wrong, such as "*.JPEG"; easy to fix:

  $ chext .JPEG .jpg

This script is careful to use the Z-Shell intrinsic functions and thus avoid gratuitus process creation.  In plain talk: fast.
