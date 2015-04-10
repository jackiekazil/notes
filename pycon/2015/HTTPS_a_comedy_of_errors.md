# HTTPS: A Comedy of Errors

Speaker: Ashwini Oruganti
Talk link: https://us.pycon.org/2015/schedule/presentation/372/
Fri. 04/10/2015 @ 11:30 - noon

- urllib2 does not validate SSL certificates

## Types of attacks

- Passive attacks -- they only need to listen to information
- Active attacks -- involve sending data to either party, man-in-the-middle-attack

## TLS
- HTTP/TLS/TCP/IP
- Most of this talk is about TLS
- SSL vs. TLS
    - SSL is old and busted and shouldn't be used anymore.
    - TLS released in 2008, 1.2
    - TLS has superseceded SSL

## Trusting the internet
- Auth: Certificates - allows us to identify a peer.
- Encryption: Math!

Can I trust this site?

## Public Key Infastructure
Site owner gets Cret
Signed by cert authority
CA= intermediary for user trust

## Connection
On connect, server sends you its certicate
client does crypto math

## Hostname Checking!
The hostname on the cert that they receive it the same that they accepted.
This is the best defense again MITM attacks.

## Encryption
Magic?

## TLS in depth (kinda)
How does session work?

### Handshake
The client tries to establish a connection w/ a 'hello' message
Then lots of decisions are made in the exchange. (more on this)

## Software
Softer that implenets TLS

* OpenSSL: most servers, non-broswer clients
* BoringSSL:
* Secure Transport

* NSS:
* (more)

### FLAWS

All these implementations have a lot of flaws in the way that they are implemented and their APIS.

They are all implemented in C & C++.

Heartbleed (OpenSSL 2014)

left certs signed certs
(Secure Transport 2001, MS CryptoAPI 2002)

#### API Design Flaws
The API is not a good example. There are too many custom settings... remember all those decisions that I talked about earlier? Now, users can use the API to make *BAD* decisions.

## Problems w/ HTTPS

### Cookie Stealing

![17073613836_0082ff78c1_k](https://cloud.githubusercontent.com/assets/166734/7091496/15d655b2-df78-11e4-82d0-862ea92216cb.jpg)

You can set a secure flag on cookies, to prevent from cookie stealing, but many developers forget to do this.

If you do set the secure flag you can still have cookies overwritten. So, secure cookies are not resistant either.

### Really?

We train people to click through this security issues.

![16479435063_b6bdb02348_k](https://cloud.githubusercontent.com/assets/166734/7091501/18c3b6a2-df78-11e4-932a-ad6ad66c1bab.jpg)


## Is urllib2 really bad?

Requests library will throw an error if it has a bad certificate, but urllib2 doesn't have it.

## Things are getting better...

More eyes on OpenSSL

[pyca/cryptography](https://github.com/pyca/cryptography)
cryptography is a package designed to expose cryptographic primitives and recipes to Python developers.
https://cryptography.io/

[pyca/tls](https://github.com/pyca/tls)
A pure Python implementation of the Transport Layer Security protocol version 1.2, using existing libraries for crypto math.

## Resources

https://www.ssllabs.com/

https://hynek.me/articles/hardening-your-web-servers-ssl-ciphers/

Test your certs against servers with bad certs

https://www.feistyduck.com/books/bulletproof-ssl-and-tls/

http://www.bookdepository.com/The-Tangled-Web-Michal-Zalewski/9781593273880?redirected=true&utm_medium=Shopping&utm_campaign=ShoppingUs&utm_source=US&utm_content=The-Tangled-Web

https://www.crypto101.io/

## Thank you

https://twitter.com/@_ashfall_

IRC: #crypotography-dev on freenode
