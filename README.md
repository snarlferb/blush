# blush

### Contributing
I'm looking for like-minded people to collaborate with. Feel free to clone and make pull requests as you please. Contributors can create their own branches or use default. We are in the early stages of spitballing ideas, and theres nothing terribly serious going on yet—if you want to get the ball rolling and start a conversation, then i would be delighted to join you in that process.

### Preface
I need to have a shell that's as fast as mksh, but w/ some of the same traits as bash (if someone wants to help me test/make comparisons i would appreciate it) The main reason being because i plan to use it while building Linux From Scratch, and that happens to be one of the main things that is hindering performance. As such, i need the shell to be sympathetic to its own size and speed.

## Ideas to play with
- [ ] Implement the histsearch (otherwise known as "Reverse-i-search") more accurately to how it functions in bash, within the same line; and that way it doesnt submit lines for each character.
- [ ] Automatic line editing and buffering, with the ability to recall previous commands from history, edit them before execution, and search through command history using shortcuts like Ctrl+R for reverse-i-search.
- [ ] Buffering refers to how the shell handles the input before it's executed. Typically, when you paste multiple lines of code or commands into a shell with buffering enabled, it retains those lines in an input buffer, allowing you to edit or review them before submitting them for execution.
- [ ] Commands to consider adding: caller, compgen (maybe), compopt (maybe), coproc, cpio (i just like this command, even as a separate idea), declare (maybe), logout, readarray, shopt...
- [ ] **Panels**: Why would you want to toggle normal mode from a shell that is suppose to be for running commands directly? Instead the normal mode should be a simplification upon commands, that is, a constant layer that you have the option of customizing yourself, like `Transformed<command> : _B_`... The transformed commands being equivalent to a binding target sequence (e.g., `"\C-d"`), and setting each simplification to the binding action (e.g., `_B_` or whatever)—which is for those people who dont like the default ViMode (and would presumably be found in `~/.npanelrc`)  Two other Panels are Emacs and MiMode, which may be activated upon pressing Fn (mod) key *(I'm still playing with this idea)*
- [ ] If you still want, you can use `set -o npanel` to enable or `set +o npanel` to disable it. You would also be able to use `setsw -o npanel` which lets you have it enabled in the same way as it would be in traditional command shells, effectively the ability to run `set -/+ o` from a key binding. This implies you can do the same with Insert Mode, so you can emulate the traditional feel—And wherein it can be set to whichever key (`<inspanel> : "\033OP"` or `"\033OP": "sw_to_inspanel"` or whatever it ends up looking like)
- [ ] Once we work on that, then it'll be utilized as the main shell for Linux From Scratch, which i will start making a collection of scripts for in [**temporary-link**](../../../ftemp/blob/main/README.md)
***

**pre-alpha - status**: almost ready
