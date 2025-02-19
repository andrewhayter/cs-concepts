## 📚 blogs and books:

* https://rust-unofficial.github.io/patterns/

* https://book.avr-rust.com/001-introduction.html
    
* https://nnethercote.github.io/perf-book/title-page.html

* https://rust-lang-nursery.github.io/rust-cookbook/intro.html
     
* https://smallcultfollowing.com/babysteps/
     
* https://lucumr.pocoo.org/
     
* https://www.lpalmieri.com/
     
* https://blog.yoshuawuyts.com/
     
* https://www.i-programmer.info/programming/theory.html
     
* https://www.i-programmer.info/babbages-bag/
     
* https://without.boats/blog/
    
## 📡 networking
#### 🛠️ tools:

* tokio
* impl riker actor for each socket connection
* libp2p pub/sub stack based on tokio tcp and udp with borsh and serde
* zmq pub/sub socket for async I/O event streaming like audio and video
* rpc capnp
* hyper
* juniper gql

#### 🎭 actor concepts:
* mailbox to receive async messages from other actors or other functions inside different part of the app  
* pub/sub channels for broadcasting, executing and scheduling async tasks using tokio cron scheduler 
* tokio worker green threadpool to run task in other threads using `tokio::spawn(async move{})`
* rpc capnp based communication with outside world actors to call each other methods directly 
* tokio message queue channles like mpsc and oneshot for sharing Arc<Mutex<T>>: Send + Sync + 'static between threads and different parts of the app 
* tokio event loop using `tokio::select!{}` to select an async I/O event task

#### 💡 concepts:
* distributed (replication and sharding) and decentralized concepts:
  * search, db and routing engines like elastic, cassandra and p2p kademlia: 
  * create best objective function to find the most rewarded (less cost actions) path in the network graph env (route planning) greedily using:
  * hybrid tech algorithms like NN, GA 🧬 and neurofuzzy(ANFIS)
  * gradient optimization methods like stochastic gradient descent 
  * none gradient optimization methods like GA and FA
  * graph theory and heuristic search algorithms like DAG, dijkstras, floyd, bellman, DFS, BFS and A*
  * reinforcement learning algorithms like qlearning using mdp and bellman equation with off and on policy methods based on markov decision process and markov chain
  * other algorithms using greedy, dynamic programming, backtracking, divide and conquer, recursive and brute forcing methods
  * hashmap based algos like hash tables (DHT) to find closest peers to a specific range of key inside a replication like cassandra db and p2p nodes    
  * rpc capnp for actor method based communication on two different machines like calling between smart contract actors
  * tokio tcp and udp and jobq channels for sharing Arc<Mutex<T>>: Send + Sync + 'static between actor threads in a same machine
  * actor tokio worker green threadpool and message queue for task and method broadcasting and scheduling to the pub/sub channels (tokio jobq, socket or rpc)
  * pub/sub and other zmq socket actors to broadcast from publishers to subscribers (m2m) using sockets
  * in libp2p peers can find each other using either mDNS (over LAN) or kademlia (over WAN)
  * in libp2p peers can communicate with each other based on pub/sub floodsub or gossipsub protocols on top of rpc capnp, tokio udp and tcp, websocket, webrtc, zmq like sockets (req/res, cli/srv or pub/sub) actors
 * proxy, firewall, vpns, packet sniffer and load balancer like pingora, HAproxy, v2ray and wireshark for all layers concepts:
   * v2ray and tor protocols
   * decompress encoded packet 
   * cpu task scheduling, 
   * weighted round robin dns, 
   * vector clock, 
   * event loop
   * iptables
   * zmq pub/sub
   * simd divide and conquer based vectorization
   
## 🏗️ system
  #### 💡 concepts:
  * compiler, vm using llvm and os
  * streaming of async I/O events compression and ram (buffer) algos like deflate, lz4 and snappy
  * data serialization codec and protocols like borsh, bson, serde, capnp and gql
  * runtime
  * video and audio codec, compressor and streamer like ffmpeg
  * cryptography
  * bridge between blockchains
  * language binding like writing rust code on top of apis of the compiled (.so) code in c like rust bindings to libsodium
  
## 🤖 AI
  #### 💡 SSL (Self Supervised Learning) concepts:
  - health improvement based on a pattern mining approach and semantic attributes like 
    - predicting missing part of the unseen input based on the exact style of the input 
    - reconstructing and labeling the unseen input based on the exact style of the input
  - feature or representation learning and extracting from the data itself
  - feature or representation selection using dimensionality reduction algorithms like GA, TSNE, PCA & VAE
  - extracting semantic attributes from the input for 0/1/few/n-shot learning 
  - autoregressive based sequence modeling to predict the future based on past events and behaviors
  - anomaly detection, 0/1/few/n-shot and meta learning
  - solving catastrophic forgetting problem using MemTransformer instead of MANN with NTM architecture LSTM based
  - FF algorithm as an alternative to gradient descent
 #### 🛠️ models and tools
  - Transformers (https://arxiv.org/abs/2101.12037)
  - SEER (https://arxiv.org/pdf/2103.01988)
  - VAE & GAN
  - BART (https://arxiv.org/pdf/1910.13461)
  - VISSL (https://vissl.readthedocs.io/en/v0.1.5/)
  - GNN (Graph Neural Network)
  - MemTransformer (https://arxiv.org/pdf/2006.11527.pdf)
  - Decision Transformer (https://arxiv.org/pdf/2106.01345v1.pdf)
  - TransZero (https://arxiv.org/abs/2112.08643)
  - DALLE-2 (https://arxiv.org/abs/2204.06125)
  - CLIP (https://arxiv.org/abs/2103.00020)
  - DayDreamer (https://arxiv.org/abs/2206.14176)
  - Algorithm Distillation (https://arxiv.org/abs/2210.14215)
  - You Only Live Once (https://arxiv.org/abs/2210.08863)
  - Forward-Forward Algorithm (https://www.cs.toronto.edu/~hinton/FFA13.pdf)
 #### 💡 NLP concepts:
* 🛠️ preprocessing
  - tokenization
  - Lexicon Normalization(stemming & lemmatization)
  - lowercasing
  - stopwwords removal
  - padding
* 📄 vocabulary building, word embedding, vectorization, feature extraction and semantic analysis
  - BOW(ngram based with TF-IDF normalization)
  - Word2Vec(skip-gram & CBOW based)
  - GloVe
  - GPT
  - BERT
  - BART
* 📈 models and statistical results
  - ML models like SVM, Naive Bayesian, Random Forest and Logistic Regression
  - DL models like LSTM(MLP+CNN), Transformers and Attentions
  - classification confusion matrix
  
