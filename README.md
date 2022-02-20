# nodejs
Learning advanced nodejs
Node started as a server side framework, but now a days is being used as Mobiles and IoT, Desktop applications and becoming popular among millions of users and is a larged ecosystem as of now.
Why is node successful
1. Javascript (so you can do a full stack along with node, if you know javascript
2. Non blocking event driven architecture, 
3. Single threaded

## Node architecture: V8 and livuv
Node's default VM is v8 to execute javascript code

Shipping: 
Staged: --harmony
InProgress: less stable features, can be see with this command `node --v8-options | grep "in progress"`

##### Garbage collector options: `node --v8-options | grep gc`

### v8
1. Node uses v8 via v8 c++ apis
2. Node itselft has an api that we can use in javascript that allows us to interact the file system, network, timer and other os system lib
3. Node api evantually executes c++ code using v8 object and function templates
4. Node also handles the waiting the async function for us using libuv
5. Since v8 is single threaded, so node also beocmes single threaded, coz its dependent on it to execute code
6. libuv is a c lib developed for node but it now used by some other languages too, this provides the event loop to node that makes it more powerful

1. http-parser
2. c-ares
3. OpenSSL
4. zlib

Chakra engine is product of microsoft

# REPL (Read eval print loop): type node in the cli and it works

# Event loop


