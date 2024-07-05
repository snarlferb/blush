# blush

### Contributing
I'm looking for like-minded people to collaborate with. Feel free to clone and make pull requests as you please. Contributors can create their own branches or use default. We are in the early stages and spitballing ideas, and theres nothing terribly serious going on yet; Even if you just want to get the ball rolling to start a conversation, i think it would be interesting for us to think about these things.

### Preface
I need to have a shell that's as fast as mksh, but w/ some of the same traits as bash (if someone wants to help me test/make comparisons to ksh, ksh93 and other shells i would appreciate it) The main reason being because i plan to use it while building Linux From Scratch, and that happens to be one of the main things that is hindering performance. As such, i need the shell to be sympathetic to its own size and speed. Feel free to 

## Ideas to play with
- [ ] Implement the histsearch (otherwise known as "Reverse-i-search") more accurately to how it functions in bash, within the same line; and that way it doesnt submit lines for each character.
- [ ] Automatic line editing and buffering, with the ability to recall previous commands from history, edit them before execution, and search through command history using shortcuts like Ctrl+R for reverse-i-search.
- [ ] Buffering refers to how the shell handles the input before it's executed. Typically, when you paste multiple lines of code or commands into a shell with buffering enabled, it retains those lines in an input buffer, allowing you to edit or review them before submitting them for execution.
- [ ] Commands to consider adding: caller, compgen (maybe), compopt (maybe), coproc, cpio (i just like this command, even as a separate idea), declare (maybe), logout, readarray, shopt...
- [ ] Vi Mode, or having switchable modes (i call panels) never quite felt right, but i suppose its because theres no indication of whats going on like there is in an editor. So to me it doesnt feel like it translates. As such we should think about how to make it work the way we want, if we do intend to change it in some way.
- [ ] New Idea: Replace Vi Mode with Mimode- i.e. My own interpretation of what i would use as someone coming from Vi but who is looking for something practical, that actually translates in the context of the shell. This just may mean that we have interesting key bindings and key combos, or it may mean something else, I dont know. Its something to think about as we go.
- [ ] We also have every compiler ever conceived of since 1975 in Build.sh, but no QBE. Can we remove Borland and Digital Mars and add QBE atleast, i think we should. There's other things too-but one step at a time.
- [ ] Once we work on that, then it'll be utilized as the main shell for Linux From Scratch, which i will start making a collection of scripts for in [**temporary-link**](../../../ftw/blob/main/README.md)
***

