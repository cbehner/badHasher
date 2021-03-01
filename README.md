# badHasher

I created two docs-

  * one containing tests, executed, with expected and actual output [here](https://github.com/cbehner/badHasher/blob/main/tests.docx)   
  * and one containing issues [here](https://github.com/cbehner/badHasher/blob/main/issues.docx)
  
My general philosophy was to write and execute a General test that covered the ports, a happy path test that found a lot of bugs, negative tests covering all endpoints, and then some simultaneous connection tests. I logged issues in the issues doc.

I probably spent too much time trying to figure out what the hasher was actually doing, but when I couldn't figure it out after a while, I moved on. 
I did see some hints though, I took this note - *decoding the base64 encoded string returns jibberish, I can't figure out what it's doing, but if
key was not "password" or data was invalid it would return the same hash, so maybe a hashed error*
