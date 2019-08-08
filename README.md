# pb-sokoban
A Sokoban game for PocketBook eReaders based on <http://pocketbook-free.sourceforge.net>

It is licensed under the GNU GPL Version 2.0
## Building
1. Clone <https://github.com/pocketbook/SDK_6.3.0/tree/5.19> and set it up as described
2. Configure with `cmake -DCMAKE_TOOLCHAIN_FILE=$SDK_DIR/SDK-$ARCHITECTURE/share/cmake/arm_conf.cmake -DCMAKE_BUILD_TYPE=Release`, replacing `$SDK_DIR` and `$ARCHITECTURE` accordingly
3. Build with `make`
4. Connect reader via USB and mount the internal storage
5. Copy pb-sokoban.app to applications/pb-sokoban.app
6. Extend your language file (e. g. system/language/en.txt) for a nicer menu entry:
```
English
@Pb-sokoban=Sokoban
```
