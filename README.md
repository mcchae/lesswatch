lesswatch
=========

lesswatch is a small utility which is watching less files recursively at every 3 second.
If one or more less file is changed or created then compile it with lessc compiler.

lesswatch 는 작은 유틸리티로서 매 3초마다 (-p 옵션으로 변경 가능합니다) less 파일을
조사하여 변경되거나 생성된 less 파일을 lessc 컴파일러로 컴파일하는 기능을 제공합니다.

Usage: ./lesswatch [options] top_root
	watch less file recursively and compile if less file changed
	options:
	-h, --help : print this help message
	-p | --period second : every watch period (default is 3 second)
	-n | --no_recursive : do not check subfolders resively
	-v --verbose: verbose mode set

example)

./lesswatch ~/workjs
==> watching $HOME/workjs folder and less file recursively and compile it
  if less file is changed or created (do not check deleted at now).
