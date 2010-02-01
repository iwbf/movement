[latest-release]: https://github.com/iwbf/movement/releases/latest
[layout-def_37th]: https://github.com/iwbf/movement/blob/main/layout/def.cfg#L37

## Movement Configs

### Install
1. Download the latest version from the [releases][latest-release] page.
2. Extract the `/movement/` folder to your `/csgo/cfg/` game directory.

### Tweak
1. Open the `/movement/layout/def.cfg` file.
2. Edit an alias in the [37th line][layout-def_37th] w/ your actual mouse wheel bindings.
    * If you don't have them, replace it w/ `unbind` command.
3. Open the `/csgo/cfg/autoexec.cfg` file.
    * If you don't have one, create then.
    * Append w/ `exec movement/lib/include.cfg` command.
    * Append w/ needed definitions — `include__std_def`, `include__hsw_def`, etc.

### Definitions
* Root `/movement/`
  * include__std_def
    * LongJump
    * CrouchJump
    * MiniJump
    * JumpBug
    * Nulls
  * include__std_wj
    * WeirdJump
  * include__std_lag
    * LadderGlide
* Half-SideWays `/movement/hsw/`
  * include__hsw_def
    * LongJump
    * CrouchJump
    * MiniJump
    * Nulls
  * include__hsw_lag
    * LadderGlide
* GOKZ `/movement/gokz/`
  * include__gokz_def
    * TP on course start
    * Danvari technique

### Miscellaneous
#### Layout `/movement/layout/`
Includes binding layouts, you can create your own and `exec` them in `autoexec.cfg`.

#### Library `/movement/lib/`
Includes aliases used internally inside other modules.
> *You don't have to be aware of this one as an end user.*
