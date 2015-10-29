# A demo Node/Express 4 app that gets A+ on the Qualys SSL Labs SSL Server Test

This app is fairly boring right now, since the authors patched node itself to implement the correct settings.

## Usage

Requires **node 4.2 +**

npm install .

Add your certs to /ssl. The following are expected:

 - Private key `example.com.private-key`
 - Certificate `example.crt`
 - CA certificate bundle `example-ca.crt`

Start the server:

    node bin/www

And visit https://localhost:3000/

Visit [Qualys SSL Labs SSL Server Test](https://www.ssllabs.com/ssltest)

Clear the cache for your site if there's an existing entry. This will initiate a new scan.

As of 2015 10 28 this Express 4 app passed the scan with A+ result.

## License

MIT

## Authors

Mike MacCana <mike@certsimple.com> @mikemaccana
