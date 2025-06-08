[
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Venesol - La moneda digital de Venezuela</title>
  <style>
    body { font-family: sans-serif; text-align: center; padding: 2rem; background: #fffbe6; color: #333; }
    header img { width: 100px; margin-bottom: 1rem; }
    .btn { background: #f1c40f; color: #000; padding: 0.75rem 1.5rem; margin: 0.5rem; border: none; cursor: pointer; font-size: 16px; border-radius: 8px; }
    .section { margin: 2rem auto; max-width: 600px; text-align: left; }
    footer { margin-top: 3rem; font-size: 0.85rem; color: #777; }
  </style>
  <script>
    async function addVENESOL() {
      try {
        await window.ethereum.request({
          method: 'wallet_watchAsset',
          params: {
            type: 'ERC20',
            options: {
              address: '0x978f0De8187BB5dFcD11B470E54f2F8417676693',
              symbol: 'VEN',
              decimals: 18,
              image: 'https://gateway.pinata.cloud/ipfs/QmYv4XZb1AbcQJpDgE1Q6g9kD9K1UMZT3sBc5x3GZqx3Rg'
            },
          },
        });
      } catch (e) {
        alert('Error al agregar el token a MetaMask');
        console.error(e);
      }
    }
  </script>
</head>
<body>
  <header>
    <img src="https://gateway.pinata.cloud/ipfs/QmYv4XZb1AbcQJpDgE1Q6g9kD9K1UMZT3sBc5x3GZqx3Rg" alt="Logo Venesol">
    <h1>Venesol (VEN)</h1>
    <p>La stablecoin venezolana para combatir la inflación. 100% respaldada. 0% inflación.</p>
    <button class="btn" onclick="addVENESOL()">➕ Agregar a MetaMask</button>
    <a href="https://quickswap.exchange/#/swap?inputCurrency=0x978f0De8187BB5dFcD11B470E54f2F8417676693&outputCurrency=USDC" target="_blank">
      <button class="btn">💱 Comprar en QuickSwap</button>
    </a>
  </header>

  <section class="section">
    <h2>¿Qué es Venesol?</h2>
    <p>Venesol es una criptomoneda estable respaldada por activos reales. Diseñada para proteger el poder adquisitivo del venezolano, es rápida, segura y descentralizada.</p>
  </section>

  <section class="section">
    <h2>Tokenomics</h2>
    <ul>
      <li><strong>Nombre:</strong> Venesol</li>
      <li><strong>Símbolo:</strong> VEN</li>
      <li><strong>Red:</strong> Polygon (Matic)</li>
      <li><strong>Contrato:</strong> 0x978f0De8187BB5dFcD11B470E54f2F8417676693</li>
      <li><strong>Suministro:</strong> 100.000.000 VEN</li>
      <li><strong>Inflación:</strong> 0%</li>
    </ul>
  </section>

  <section class="section">
    <h2>📄 Whitepaper Oficial</h2>
    <a href="https://gateway.pinata.cloud/ipfs/QmYv4XZb1AbcQJpDgE1Q6g9kD9K1UMZT3sBc5x3GZqx3Rg/whiterpaper%20VENESOL.pdf" target="_blank">Descargar PDF</a>
  </section>

  <footer>
    <p>&copy; 2025 Venesol. Todos los derechos reservados.</p>
    <p>Síguenos: @venesolcoin (Telegram, X, Instagram)</p>
  </footer>
</body>
</html>
Uploading index.html…]()
