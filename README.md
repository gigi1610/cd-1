const http = require('http');

const server = http.createServer((req, res) => {
 if (req.method === 'GET' && req.url === '/') {
    res.statusCode = 200;
    res.setHeader('Content-Type', 'text/plain');
    res.end('Olá, mundo!');
 }
});

server.listen(3000, () => {
 console.log('Servidor rodando na porta 3000');
});# cd-1
