# Bright Data SOCKS5 Proxies

[![Promo](https://github.com/luminati-io/SOCKS5-Proxies/blob/main/first-deposit-banner.PNG)](https://brightdata.com/solutions/socks5-proxies) 

## Overview
Send SOCKS5 proxy server requests using Bright Data’s Proxy Manager and enjoy seamless, high-speed scraping with Bright Data's [SOCKS5 proxies](https://brightdata.com/proxy-types/socks5-proxies), designed for versatility, anonymity, and top performance.

- **Supports TCP & UDP traffic**
- **SOCKS5 Protocol for maximum compatibility**
- **99.99% success rate**
- **Free Geo-location targeting (Country, City, State, ZIP)**

## Key Features
- **Global Coverage**: SOCKS5 proxies available in [195 countries](https://brightdata.com/locations).
- **High Success Rates**: Up to 99.99% success for scraping and data collection.
- **Fast Response**: Reliable connections with minimal latency.
- **Versatile Protocol**: Suitable for HTTP, HTTPS, FTP, and more.
- **Unlimited Scaling**: No restrictions on concurrent sessions.

## SOCKS5 Proxy Pricing

### Residential Proxies

- **Pay As You Go**: $8.4/GB, no monthly commitment required.
- **Monthly Subscriptions**:
  - **69 GB**: $7.14/GB, $499/month.
  - **158 GB**: $6.3/GB, $999/month.
  - **339 GB**: $5.88/GB, $1999/month.
  - **Enterprise Plans**: Custom pricing and solutions available for large-scale operations.

 ### ISP Proxies

- **Pay As You Go**: $1.8/IP, no monthly commitment required.
- **Monthly Subscriptions**:
  - **10 IPs**: $1.8/IP, $18/month.
  - **100 IPs**: $1.45/IP, $145/month.
  - **500 IPs**: $1.4/IP, $700/month.
  - **1,000 IPs**: $1.3/IP, $1,300/month.
  - **Enterprise Plans**: Custom pricing and solutions available for operations requiring more than 1,000 IPs.
 
### Datacenter Proxies

- **Pay As You Go**: $1.40/IP, no monthly commitment required.
- **Monthly Subscriptions**:
  - **10 IPs**: $1.40/IP, $14/month.
  - **100 IPs**: $1.00/IP, $100/month.
  - **500 IPs**: $0.95/IP, $475/month.
  - **1,000 IPs**: $0.90/IP, $900/month.
  - **Enterprise Plans**: Custom pricing and solutions available for operations requiring more than 1,000 IPs.

Sign up and receive a dollar-for-dollar match on your first deposit, up to $500!

## Getting Started with SOCKS5 Proxies
1. **Start Free Trial**: No credit card required.
2. **Integration**: Use Bright Data Proxy Manager or APIs to manage SOCKS5 proxies.
3. **Supported Platforms**: Easily configure SOCKS5 proxies in Python, Node.js, cURL, and more.

## Code Examples

### Python

```python
import requests

proxy = {
    "http": "socks5h://[your username]:[your password]@brd.superproxy.io:22228",
    "https": "socks5h://[your username]:[your password]@brd.superproxy.io:22228"
}

response = requests.get("https://geo.brdtest.com/mygeo.json", proxies=proxy)
print(response.json())
```

### Node.js

```node.js
const request = require("request-promise");

const options = {
  url: "https://geo.brdtest.com/mygeo.json",
  proxy: "socks5h://[your username]:[your password]@brd.superproxy.io:22228",
};

request(options)
  .then(function (response) {
    console.log(response);
  })
  .catch(function (err) {
    console.error(err);
  });
```

### cURL

```shell
curl -x socks5h://brd.superproxy.io:22228 \
     --proxy-user [your username]:[your password] \
     "https://geo.brdtest.com/mygeo.json"
```

## Use Cases
Explore the versatility of SOCKS5 proxies for various industries:

- [**eCommerce**](https://brightdata.com/use-cases/ecommerce): Track product pricing, reviews, and availability from multiple regions.
- [**Social Media**](https://brightdata.com/use-cases/social-media-for-marketing): Monitor trends, engagement, and competitor activity anonymously.
- [**Travel**](https://brightdata.com/use-cases/travel): Compare travel deals across countries and regions with precise geo-targeting.
- [**Financial Services**](https://brightdata.com/use-cases/financial): Collect real-time market data and analyze trends securely.

---

## FAQ

### What is the SOCKS5 Proxy Protocol?
SOCKS5 is a versatile proxy protocol that routes network packets between a client and a server via a proxy. It supports both TCP and UDP connections, enabling a wide range of applications, such as web scraping, bypassing restrictions, and enhancing anonymity.

### How does SOCKS5 differ from HTTP proxies?
SOCKS5 operates at a lower level than HTTP proxies, allowing it to handle a broader range of traffic types, including HTTP, HTTPS, FTP, and SMTP. It also provides higher anonymity by not modifying network packets.

### How can I use SOCKS5 proxies with Bright Data services?
Bright Data supports SOCKS5 on its Residential, Datacenter, and ISP proxy networks. To use SOCKS5:
1. Configure your application to use `brd.superproxy.io` on port `22228`.
2. Use your Bright Data credentials for authentication.
3. Ensure remote DNS resolution with the `socks5h://` protocol.

### What is the default port for SOCKS5 proxies?
The default SOCKS5 proxy port for Bright Data is `22228`. Note that standard ports for HTTP (`22225`) and HTTPS (`22226`) are not applicable for SOCKS5 connections.

### What are the benefits of using SOCKS5 proxies?
SOCKS5 proxies offer:
- **High Anonymity**: Masks your IP for secure and private connections.
- **Versatility**: Handles multiple traffic types, including HTTP, HTTPS, FTP, and more.
- **Bypass Restrictions**: Overcome geo-blocks, firewalls, and censorship.
- **TCP and UDP Support**: Suitable for a wide variety of use cases.
- **Reliable Performance**: High uptime and low latency with Bright Data's robust infrastructure.

### How can I ensure the best performance with SOCKS5 proxies?
To optimize performance:
1. Use domain names as targets instead of IPs.
2. Configure remote DNS resolution with the `socks5h://` protocol.
3. Use [Bright Data’s Proxy Manager](https://brightdata.com/products/proxy-manager) for advanced features like IP rotation and request optimization.

### Can I perform geo-targeting with SOCKS5 proxies?
Yes, Bright Data's SOCKS5 proxies support precise geo-targeting. You can target specific countries, cities, states, ZIP codes, and ASNs by modifying your username (e.g., `username-country-us` for the United States).

### Are SOCKS5 proxies compliant with Bright Data's policies?
Yes, Bright Data's SOCKS5 proxies adhere to GDPR and CCPA regulations, ensuring compliance and ethical data usage. Follow all guidelines provided to maintain compliance.

### What are the limitations of using SOCKS5 proxies?
- **IP Restrictions**: Only domain names are supported; direct IP requests are blocked.
- **Port Restrictions**: Must use port `22228` for SOCKS5 connections.
- **Remote DNS Resolution**: Requires `socks5h://` protocol for compliance.
- **Target Ports**: Supports only ports above `1024`.
