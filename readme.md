# HTTP vs HTTPS Traffic Analysis Using Wireshark

## Overview

This project explores the differences between HTTP and HTTPS traffic using Wireshark. The purpose of the analysis is to understand how data travels across a network, how unencrypted communication can be inspected, and how HTTPS protects information through TLS encryption.

By capturing and analyzing network packets, this project demonstrates the importance of secure communication protocols and provides practical experience with packet analysis using Wireshark.

## Objectives

* Capture and analyze HTTP traffic.
* Capture and analyze HTTPS traffic.
* Understand the TLS handshake process.
* Use Wireshark display filters to isolate specific traffic.
* Compare the security characteristics of HTTP and HTTPS.
* Document findings in a professional manner.

## Tools Used

* Wireshark
* Google Chrome / Mozilla Firefox
* Windows Operating System

## Display Filters Used

```text
http
http.request
http.response
tcp.port == 80
tls
tls.handshake
tls.handshake.type == 1
tls.handshake.type == 2
```

## Project Structure

```text
HTTP-vs-HTTPS-Traffic-Analysis/
│
├── README.md
├── Report.pdf
├── Screenshots/
│   ├── HTTP_Capture.png
│   ├── HTTP_Filter.png
│   ├── HTTPS_Capture.png
│   ├── TLS_Handshake.png
│   ├── Client_Hello.png
│   └── Server_Hello.png
```

## Key Findings

* HTTP traffic is transmitted without encryption.
* Information contained in HTTP packets can be viewed directly.
* HTTPS encrypts communication using TLS.
* TLS handshake establishes a secure connection before data exchange begins.
* Encrypted HTTPS traffic cannot be easily read from packet captures.

## Learning Outcomes

Through this project, I gained hands-on experience with network traffic analysis, packet inspection, display filtering, and TLS communication. The project also improved my understanding of web security concepts and practical network monitoring techniques.


