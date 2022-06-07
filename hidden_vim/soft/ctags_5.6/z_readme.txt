1) install

./configure --prefix=/home/caohaijun/usr/local/ctags-5.6 && make && make install

in my_bashrc add: export PATH=/home/caohaijun/usr/local/ctags-5.6/bin:$PATH

"which ctags" to check 


2) usage

ctags -R --sort=1 --c++-kinds=+p --fields=+iaS --extra=+q --language-force=C++ -f cpp .

--c++-kinds=+p //add tags with function prototype
--fields=+iaS  //add tags for inheritance, access, function Signature (param table )
--extra=+q    // add class label for class member
