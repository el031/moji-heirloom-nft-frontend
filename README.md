j# moji-heirloom-nft-frontend
# moji-heirloom-nft-frontend
![Moji Heirloom Badge](./moji031/moji0.31logo.png)
Frontend application for **Moji0.31 Heirloom NFTs**.

This project allows users to:
- Connect their crypto wallet (e.g., MetaMask)
- Mint heirloom NFTs
- View and manage their collection
- Access exclusive Moji0.31 member content

---

## 🚀 Tech Stack
- **Framework:** Next.js (React)
- **Styling:** Tailwind CSS
- **Blockchain:** Polygon / EVM compatible
- **Deployment:** Vercel

---

## ⚙️ Installation

```bash
# Clone the repository
git clone https://github.com/your-username/moji-heirloom-nft-frontend.git
cd moji-heirloom-nft-frontend

# Install dependencies
npm install
npm run dev
http://localhost:3000
npm run build
npm run start
NEXT_PUBLIC_API_URL=https://api.moji031.xyz
NEXT_PUBLIC_WALLET_CONNECT_KEY=0x8a9d02a8a716b8941dfaed6b6dd4360002e7d8b8
NEXT_PUBLIC_PROJECT_ID=moji031
## License
This project is licensed under the [MIT License](./LICENSE).curl -X POST "https://api.pinata.cloud/pinning/pinFileToIPFS" \
-H "pinata_api_key:  7fa0afde86c8fe00b0d5     " \
-H "pinata_secret_api_key:  95ff1f364d8bc47da6555613f4fb6f2e206346846134c862dcea6de99c02370c " \
-F "file=@./public/moji0.31logo.png"

# Moji0.31 

Website: https://moji031-pukjedmfn-electras-projects-331853b6.vercel.app

## Assets- Logo: public/moji0.31logo.png
- Badge: file_000000008ba862469defba236638a9d5.png

## Deployment
- GitHub Repository: moji-heirloom-nft-frontend
- Vercel Deployment: [https://moji031-pukjedmfn-electras-projects-331853b6.vercel.app]

## NFT Metadata
- JSON file: data/metadata.json
- IPFS Pinning: Pinata / NFT.Storage


{"name": "Moji0.31 Heirloom Badge",
  "description": "Official badge for verified Moji0.31 NFT owners. Grants access to heirloom assets and private membership.",
  "image": "https://   moji031-pukjedmfn-electras-projects-331853b6.vercel.app/moji031/file_000000008ba862469defba236638a9d5.pngfile_000000008ba862469defba236638a9d5.png",
  "external_url": "https://moji031-pukjedmfn-electras-projects-331853b6.vercel.app/",
  "attributes": [
    { "trait_type": "Generation", "value": "0.31" },
    { "trait_type": "Type", "value": "Heirloom" },
    { "trait_type": "Network", "value": "Polygon" }
  ]
}

{
  "name": "Moji0.31 Heirloom Badge",
  "description": "Official badge for verified Moji0.31 NFT owners. Grants access to heirloom assets and private membership.",
  "image": "ipfs://<bafybeifvzcilybfaktkmefh65teofulyb2y4qlmygz7gfk3xeq4cucvhtq>",
  "external_url": "https://moji031-pukjedmfn-electras-projects-331853b6.vercel.app/",
  "attributes": [
    { "trait_type": "Generation", "value": "0.31" },
    { "trait_type": "Type", "value": "Heirloom" },
    { "trait_type": "Network", "value": "Polygon" }
  ]
}
