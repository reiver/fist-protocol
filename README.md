# Fist Protocol



## Design

The **fist protocol** is inspired by the **finger protocol** and the ways which **finger** was used people.

**finger** is said to have be created back in 1971.

I was using **finger** in the 1990s — and maintained my own **finger** (`.plan`) file.
My **finger** (`.plan`) file backn then contained:
* contact information,
* URLs to my presence on other parts of the Internet,
* a short biography,
* a journal,
* articles,
* jokes,
* a bunch of ASCII art.

I stored all that information in separate files, which were compiled into a **finger** `.plan` file. 

Back then I (and I suspect most people) accessed **finger** from a terminal or terminal emulator, connected to a Unix system, by invoking command similar to:
```
finger username
```
(Here `username` would be replaced by the person's username on that Unix system.

So, for example:
```
finger joeblow
```
Or:
```
finger dariush
```

### Finger Protocol Advantages

Some desirable qualities of the 1970s era **finger protocol** are:

* ✅ it is a **human-readable** protocol
  * rather than just a programmer-readable or machine-readable protocol
* ✅ the protocol is **simple enough** for even a more junior software developer to be able to understand it
* ✅ the protocol and default data-format are **simple enough** for a competent software developer to be able to create a (simple) working **client** as a weekend project
  * ✅ if the default data-format is dumped to a terminal or terminal emulator it is human-readable
* ✅ the protocol is **simple enough** for a competent software developer to be able to create a (simple) working **server** as a weekend project
* ✅ all of a (single) user's content is provided as a **single download**
* ✅ a client could make a request from a server for a user who is _not_ (necessarily) local to that server
* ✅ key-value pairs which are in a format that is **human-readable**, **programmer-readable**, and **machine-readable**.

### Finger Protocol Disadvantages

Some undesirable qualities of the 1970s era **finger protocol** are:

* when a client receives a response from a server, it does not know whether it received all the data or not, as, for example, the network connection could have been disconnected prematurely, but there is no way to detect this,
* there is no _tamper detection_,
* there is no way to determine whether the finger (`.plan`) file was actually from the user whose content was requested,
* there is no privacy,
* the entire finger (`.plan`) file must be download each time, even if the exact same finger (`.plan`) file was previously downloaded,
* identity is strictly tied to an Internet domain,
* there is no official way of segmenting the download (into sub-pages).


