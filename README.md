# Ping
This is a proyect for make a ping with analysis functionalities.

## Requirements
This only works on a linux os and you need to have installed the following dependencies:
<ul>
	<li>Go compiler</li>
	<li>UPX</li>
</ul>

## Instalation
Clone this repository and execute the build.sh script
```console
$ git clone https://github.com/AkaliRep/ping-rawsockets
$ ./build.sh
```

## Usage
You just need to run the ping executable generated by build.sh script.<br/>
The os is calculated based on TTL, by default linux systems have 64TTL and windows systems 128TTL. This is not 100% accurate.
```console
$ ./ping -h 192.168.0.1
Sending ping to: 192.168.0.1
---------------------------------
Time: 0.635ms	TTL: 64 (Probably OS: Linux)
Time: 0.514ms	TTL: 64 (Probably OS: Linux)
Time: 0.474ms	TTL: 64 (Probably OS: Linux)
Time: 0.489ms	TTL: 64 (Probably OS: Linux)
Total sent: 4	Total recived: 4	Total lost: 0	100.00% Recieved
```

You can see the help by typing -help
```console
$ ./ping -help
Usage of ping:
  -c int
    	Number of packets you want to send (default 4)
  -h string
    	Host you want to ping (default "127.0.0.1")
```

## Incoming Features
I have in mind adding the following features:
<ul>
	<li>Port scan</li>
	<li>DNS Resolve</li>
</ul>