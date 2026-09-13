# HTTPS SSL

Scripts and configuration for setting up DNS subdomains, SSL termination
on HAProxy, and HTTP-to-HTTPS redirection.

## Files

- 0-world_wide_web: Bash script that queries DNS records for subdomains
  using dig and awk, and prints their record type and destination.
- 1-haproxy_ssl_termination: HAProxy configuration file
  (/etc/haproxy/haproxy.cfg) configured for SSL termination on port 443.
- 2-redirect_http_to_https: HAProxy configuration file
  (/etc/haproxy/haproxy.cfg) configured to redirect HTTP traffic to
  HTTPS with a 301 response.
