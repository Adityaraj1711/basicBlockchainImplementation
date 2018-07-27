# basicBlockchainImplementation
implementing a basic Blockchain model using GoEthereum.

<h1>
  required steps
</h1>
<hr>
<ul>
    <li>install goethereum</li>
    <li>register a goethereum account</li>
    <li>Create Autonomous blockchain</li>
    <li>perform transaction internally</li>
</ul>


<h1>
  Step 1
</h1>
<hr>
<li>
    git clone goethereum:
    <li>&nbsp;git clone https://github.com/ethereum/go-ethereum</li> 
</li>
<li>
  cd go_ethereum\
</li>
<li>
  ls
</li>
<li>
  git tag <p>(for diffrent versions) Now creating a branch of latest version</p>
</li> 
<li>
  git checkout tags/v1.6.7 -b EdurekaEthereum1.6.7
</li>
<li>git branch</li>
<li>Download Go language<p>sudo tar -xvf go1.8.3.linux-386.tar.gz  (or whatever the version you ot of Go)</p></li>
<li>Now move it to specific location</li>
<li>type commands in terminal
  <hr>
  <pre>
    sudo mv go/usr/local
    ls
    cdc
    #now open new terminal
    cd  
    sudo gedit.bashrc         (for adding enviornment variables)
  </pre>
</li> 
<li>
   <pre>
    add these lines
    export GOROOT = /usr/local/go
    export GOPATH = $HOME/Projects/proj1
    export PATH = $GOPATH/bin:$ GOROOT/bin:$PATH
 now in terminal:
  source .bashrc
  new terminal :
    cd go-ethereum
    go version
    make all                (to build target file)
 
   </pre>
   
</li> 
<h1>
Step 2
</h1>
<hr>
<pre>
  (creating a genesis block)
  cd go-ethereum
  mkdir genesis
  cd genesis/
  gedit genesis3.json
  
  {
    "nonce":"0x3",
    "timestamp":"0x0",
    "parentHash":"0x0000000000000000000000000000",
    "extraData":"0x0",
    "gasLimit":"0x4c4b40",
    "difficulty":"0x400",
    "mixhash":"0x000000000000000000000000000",
    "coinbase":"0x0000000000000000000",
    "alloc":{
    }
  }
  
  # understanding  the terms
   parenthash: Hash code of parent
   extra data: extra 32 bit to pass
   difficulty : it is the measure of difficulty to mine data
   mixhash : kept fixed throughout blockchain
   combination of nonce and mixhash are called as proof of work
   we need to identify te value of nonce
   gas limit is the limit
   alloc is used to define a list of prefilled wallet
  
</pre>
<h1>Step 3</h1>
<hr>




















