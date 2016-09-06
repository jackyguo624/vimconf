## The steps for customizing vim
1. Install x11-dev 

2. Download this vim && compile 
```bash
    cd vim/
    ./configure --with-features=huge --enable-pythoninterp --enable-rubyinterp --enable-luainterp --enable-perlinterp --with-python-config-dir=/usr/lib/python2.7/config/ --enable-gui=gtk2 --enable-cscope --prefix=/usr
    make
    make install
```
3. replace .vimrc 

4. Standardc++ complete:  
    generate c++ tags with ctags && add in tags of.vimrc 

5. C++ snippet:   
    Put cpp.snippets to '~/.vim/bundle/ultisnips/mysnippets/cpp.snippets' && let g:UltiSnipsSnippetDirectories=["mysnippets"] 

6. YouCompleteMe: Intelligent and compiler Complete and contains 4 and 5

    1. Install clang-completer 
    ```bash
    cd ~/.vim/bundle/YouCompleteMe
    ./install.py --clang-completer
    ```
    2. Put .ycm_extra_conf.py under project



## Usage for cpp coding and debugging
1. Navigate: nerdTree ;fl
2. Multi_tab: ;bl 
3. Compile: Write CMakeList.txt && :!cmake CMakeList.txt 
4. Make and run: ;g 
