# lua-resty-fileinfo

`lua-resty-fileinfo` is a file information library implementing LuaJIT bindings to `libmagic`.

## Hello World with lua-resty-fileinfo

```lua
local fileinfo = require "resty.fileinfo"
fileinfo"a.txt"
```

This will return string containing `ASCII text`. But there are other information available as well.

## Installation

Just place [`fileinfo.lua`](https://github.com/bungle/lua-resty-fileinfo/blob/master/lib/resty/fileinfo.lua) somewhere in your `package.path`, preferably under `resty` directory. If you are using OpenResty, the default location would be `/usr/local/openresty/lualib/resty`.

### Compiling and Installing libmagic C-library

Consult you operating system about installing this. Or compile from the sources.

### Using LuaRocks or MoonRocks

If you are using LuaRocks >= 2.2:

```Shell
$ luarocks install lua-resty-fileinfo
```

If you are using LuaRocks < 2.2:

```Shell
$ luarocks install --server=http://rocks.moonscript.org moonrocks
$ moonrocks install lua-resty-fileinfo
```

MoonRocks repository for `lua-resty-fileinfo` is located here: https://rocks.moonscript.org/modules/bungle/lua-resty-fileinfo.

## Lua API

TBD

## License

`lua-resty-fileinfo` uses two clause BSD license.

```
Copyright (c) 2014, Aapo Talvensaari
All rights reserved.

Redistribution and use in source and binary forms, with or without modification,
are permitted provided that the following conditions are met:

* Redistributions of source code must retain the above copyright notice, this
  list of conditions and the following disclaimer.

* Redistributions in binary form must reproduce the above copyright notice, this
  list of conditions and the following disclaimer in the documentation and/or
  other materials provided with the distribution.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR
ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

