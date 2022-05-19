# Fist Protocol

## Design

The **fist protocol** is inspired by the **finger protocol** and the ways which **finger** was used people.

**finger** is said to have be created back in 1971.

I was using **finger** in the 1990s — and maintained my own **finger** (`.plan`) file.
My **finger** (`.plan`) file contained:
* contact information,
* URLs to my presence on other parts of the Internet,
* a short biography,
* a journal,
* articles,
* jokes,
* a bunch of ASCII art.

Back then I (and I suspect most people) accessed **finger** from a terminal or terminal emulator, connected to a Unix system, by invoking command similar to:
```
finger username
```
(here `username` would be replaced by the person's username on that Unix system.

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
  * rather than just a programmer-readable or machine-readable protocol,
* ✅ the protocol is **simple enough** for even a more junior software developer to be able to understand it
* ✅ the protocol and default data-format is **simple enough** for a competent software developer to be able to create a (simple) working **client** as a weekend project
* ✅ the protocol is **simple enough** for a competent software developer to be able to create a (simple) working **server** as a weekend project
* ✅ all of a user's content was provided as a **single download**

### Finger Protocol Disadvantages

Some undesirable qualities of the 1970s era **finger protocol** are:

* when a client receives a response from a server, you do not know whether you received all the data or not, or if the connection was disconnected prematurely,
* there is no _tamper detection_,
* there is no privacy.
