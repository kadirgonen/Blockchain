# Blockchain

We built a blockchain recently on my this work.
Since then, I've added a project on my github account - one containing proof of work blockchain and the other containing proof of stake blockchain.

So, now we know how to build a blockchain and how the two most popular consensus mechanisms work. But blockchains themselves need to be propagated across peers.

This means - communication across multiple peers. In this example, I wanted to show that.
You need to open up multiple terminals to see this happen.

1. 1st terminal - `go run main.go -secio -l 10000`
2. 2nd terminal - `go run main.go -l 10001 -d /ip4/127.0.0.1/tcp/10000/ipfs/QmZ8NayvdXc2U2A1cwh9qGaHK7uxXXVrZQEYwDqbfFydfj -secio`
3. 3rd teminal - `go run main.go -l 10002 -d /ip4/127.0.0.1/tcp/10001/ipfs/QmRAj9JJVKRJmWHbDKzvzKDVVFPWxuWYio3bPym4SgGPgF -secio`
