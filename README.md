# TicketSafes
<<<<<<< HEAD
NTF Ticketing Marketplace
=======

Sistema de venta y gestión de tickets para eventos en Arbitrum.

## Descripción

TicketSafes es una plataforma descentralizada para la venta y gestión de tickets de eventos, construida sobre la red Arbitrum. El sistema incluye características avanzadas como:

- Sistema anti-scalping
- Sistema de reputación de usuarios
- Precios dinámicos basados en la demanda
- Subastas de tickets
- Sistema de reembolsos
- Verificación de usuarios

## Tecnologías

- Solidity 0.8.19
- Hardhat
- OpenZeppelin Contracts
- Ganache (para desarrollo local)

## Configuración del Entorno

### Requisitos Previos

- Node.js (versión 16 o superior)
- npm o yarn
- Ganache (para desarrollo local)

### Instalación

1. Clonar el repositorio:
```bash
git clone https://github.com/tu-usuario/ticketsafes.git
cd ticketsafes
```

2. Instalar dependencias:
```bash
npm install
```

3. Configurar variables de entorno:
Crear un archivo `.env` en la raíz del proyecto con las siguientes variables:
```
ARBITRUM_RPC_URL=tu_url_rpc_arbitrum
PRIVATE_KEY=tu_clave_privada
PROJECT_ID=tu_id_proyecto_infura
COINMARKETCAP_API_KEY=tu_api_key_coinmarketcap
ETHERSCAN_API_KEY=tu_api_key_etherscan
```

## Desarrollo Local

1. Iniciar Ganache:
```bash
ganache --port 8546
```

2. Compilar contratos:
```bash
npx hardhat compile
```

3. Desplegar contratos en red local:
```bash
npx hardhat run scripts/deploy.js --network development
```

## Redes Soportadas

- **Development**: http://127.0.0.1:8546 (Ganache)
- **Arbitrum**: Red principal de Arbitrum
- **Arbitrum Sepolia**: Red de pruebas de Arbitrum

## Configuración de Redes

### Development (Ganache)
- Chain ID: 1337
- Gas Limit: 6721975
- Gas Price: 20000000000
- Hardfork: shanghai

### Arbitrum
- Chain ID: 42161
- Gas Limit: 8000000
- Gas Price: 100000000

### Arbitrum Sepolia
- Chain ID: 421614
- Gas Limit: 8000000
- Gas Price: 100000000

## Scripts Disponibles

- `npm run compile`: Compila los contratos
- `npm run test`: Ejecuta las pruebas
- `npm run deploy`: Despliega en Arbitrum
- `npm run deploy:local`: Despliega en red local
- `npm run node`: Inicia un nodo Hardhat local

## Estructura del Proyecto

```
ticketsafes/
├── contracts/           # Contratos inteligentes
├── scripts/            # Scripts de despliegue
├── test/              # Pruebas
├── artifacts/         # Artefactos de compilación
├── cache/            # Caché de compilación
└── hardhat.config.js # Configuración de Hardhat
```

## Licencia

MIT

## Características

- Venta de tickets usando ETH/WETH
- Sistema de precios dinámicos
- Sistema de subastas
- Sistema de reputación
- Sistema anti-scalping
- Interfaz de usuario moderna y responsive

## Requisitos

- Node.js v18 o superior
- Ganache v7.7.7
- Truffle v5.8.1
- MetaMask o cualquier wallet compatible con Web3

## Instalación

1. Clonar el repositorio:
```bash
git clone https://github.com/tu-usuario/ticketsafes.git
cd ticketsafes
```

2. Instalar dependencias:
```bash
npm install
cd frontend
npm install
```

3. Configurar variables de entorno:
```bash
cp .env.example .env
# Editar .env con tus configuraciones
```

4. Iniciar Ganache:
```bash
ganache --port 8545
```

5. Desplegar contratos:
```bash
truffle migrate
```

6. Iniciar el frontend:
```bash
cd frontend
npm run dev
```

## Uso

1. Conecta tu wallet (MetaMask)
2. Crea un nuevo evento
3. Compra tickets
4. Gestiona tus tickets (transferir, subastar, etc.)

## Contribuir

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## Contacto

Tu Nombre - [@tutwitter](https://twitter.com/tutwitter)

Link del Proyecto: [https://github.com/tu-usuario/ticketsafes](https://github.com/tu-usuario/ticketsafes)

## Contratos Verificados en Arbitrum

| Contrato | Dirección | Verificado |
|----------|-----------|------------|
| TicketSafe | [0xB07E16B1F5712f79120fC166daC9D22A812f6123](https://sepolia.arbiscan.io/address/0xB07E16B1F5712f79120fC166daC9D22A812f6123) | ✅ |
| MockWETH | [0xEBebB8f71FE9133EC0979BAd3886b528a9b4D68a](https://sepolia.arbiscan.io/address/0xEBebB8f71FE9133EC0979BAd3886b528a9b4D68a) | ✅ |
| PriceFeed | [0xE2A338Ff01fe8cfd77615B41a891d325fF01D1d9](https://sepolia.arbiscan.io/address/0xE2A338Ff01fe8cfd77615B41a891d325fF01D1d9) | ✅ | 
>>>>>>> 69b57a3 (Primer commit: proyecto TicketSafes listo y funcionando en Arbitrum Sepolia)
