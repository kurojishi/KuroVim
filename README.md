KuroVim
=======

my personal .vimrc, feel free to use it and modify as you wish


it uses vundle for plugin management and the init can be a bit long

for YouCompleteMe plugin and Syntastic please follow their documentation for a correct setup(use the full installation guide for all the features)
https://github.com/Valloric/YouCompleteMe
https://github.com/scrooloose/syntastic


it's still not final, it need a lot of polishing as it's pratically a fork(reorganized and heavily modified) of CrisiVim by crisidev
if you find something that can be improved or removed please set up a issue i'm open to modifications


INSTALL and SETUP
--------
be sure to have at least vim 7.3.584(needed by YouCompleteMe) compiled with +python support.
you need to clone vundle in .vim/bundle/ https://github.com/gmarik/vundle/ a :BundleInstall! will download and install all the other plugin

YouCompleteMe need to be compiled cd .vim/bundle/YouCompleteMe && ./install.sh --clang-completer 
but read the doc for more infos

GO autocomple and code checking
-----
go need a couple of software for a good autocomplete and a best syntax checking
be sure to have a propely set up $GOPATH and $GOBIN(this one generaly need to be set up in $GOPATH/bin) and to have $GOBIN in your path

then install ````go get https://github.com/nsf/gocode````, ````go get https://github.com/golang/lint````, ````go get -v code.google.com/p/rog-go/exp/cmd/godef```` and ````go get -u github.com/jstemmer/gotags```` reload your shell and check if you have these tools in your path, then everything should work fine, gocode is the autocomplete engine it's absolutely fast and complete, golint is an error checker that work with syntastic, godef is for getting the definition of a method/function/variables and gotags is for escuberant-ctags like tags that work wonders with tagbar have fun

TODO
----
-Add a spf13 like bootstrap script
