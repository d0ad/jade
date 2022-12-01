# JADE Book Trading

Multi-agent trading system

## Build agents

Requirements: 
- Java SDK version: 17
- jade.jar
- commons-codec-1.3.jar

```bash
export CLASSPATH=jade/lib/jade.jar:jade/lib/commons-codec/commons-codec-1.3.jar:out
javac --release 17 -d out src/*.java
```
## Run agents

```bash
# Start Seller Agent
java jade.Boot -gui seller:bookTrading.BookSellerAgent

# Start Byuer Agent
java jade.Boot -container -agents "buyer:bookTrading.BookBuyerAgent(The-Golden-Era)"
```
