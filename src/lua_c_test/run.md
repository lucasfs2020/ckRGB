To run the lua_test.c file, a proof of concept that shows how to run lua scripts in c, do the following steps in wsl

1a. Install lua5.2 and liblua5.2-dev through sudo apt-get install.
1b. If you are on a mac, use brew install lua
2. cd into the lua_c_test folder.
3a. Run the following command to create test_lua: gcc lua_test.c -o test_lua -llua5.2 -I/usr/include/lua5.2/.
3b. The above should only been done if you installed with apt-get. Otherwise use gcc lua_test.c -o test_lua -llua
4. Run test lua.

If you have followed the steps above, the program should callfuncscript.lua, the square function, and helloscript.lua
