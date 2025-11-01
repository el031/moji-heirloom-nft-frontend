j# moji-heirloom-nft-frontend
# moji-heirloom-nft-frontend
"image": "ipfs://<bafybeifvzcilybfaktkmefh65teofulyb2y4qlmygz7gfk3xeq4cucvhtq>",
(moji0.31logo.png)

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

## Assets- Logo:moji0.31logo.png
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
  ]o 
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
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>React Code Analyzer</title>
<style>
* { margin:0; padding:0; box-sizing:border-box; }
body { font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; line-height:1.6; color:#333; background: linear-gradient(135deg,#667eea 0%,#764ba2 100%); min-height:100vh; }
.container { max-width:1200px; margin:0 auto; padding:20px; }
.header { text-align:center; color:white; margin-bottom:30px; }
.header h1 { font-size:2.5rem; margin-bottom:10px; text-shadow:2px 2px 4px rgba(0,0,0,0.3); }
.card { background:white; border-radius:15px; padding:30px; box-shadow:0 10px 30px rgba(0,0,0,0.2); margin-bottom:20px; transition:transform 0.3s ease,box-shadow 0.3s ease; }
.card:hover { transform:translateY(-5px); box-shadow:0 15px 40px rgba(0,0,0,0.3); }
.upload-area { border:3px dashed #667eea; border-radius:10px; padding:40px; text-align:center; background:#f8f9ff; transition: all 0.3s ease; cursor:pointer; }
.upload-area:hover { border-color:#764ba2; background:#f0f2ff; }
.upload-area.dragover { border-color:#4CAF50; background:#e8f5e8; }
textarea { width:100%; min-height:200px; padding:15px; border:2px solid #ddd; border-radius:8px; font-family:'Courier New', monospace; font-size:14px; resize:vertical; transition:border-color 0.3s ease; }
textarea:focus { outline:none; border-color:#667eea; }
.btn { background: linear-gradient(45deg,#667eea,#764ba2); color:white; border:none; padding:12px 30px; border-radius:25px; cursor:pointer; font-size:16px; font-weight:600; transition:all 0.3s ease; margin:10px 5px; }
.btn:hover { transform:translateY(-2px); box-shadow:0 5px 15px rgba(0,0,0,0.2); }
.btn:active { transform:translateY(0); }
.analysis-result { background:#f8f9fa; border-left:4px solid #667eea; padding:20px; border-radius:8px; margin-top:20px; display:none; }
.component-list { display:grid; grid-template-columns:repeat(auto-fit,minmax(250px,1fr)); gap:15px; margin-top:20px; }
.component-item { background:#e3f2fd; padding:15px; border-radius:8px; border-left:4px solid #2196F3; transition:all 0.3s ease; }
.component-item:hover { background:#bbdefb; transform:translateX(5px); }
.progress-bar { width:100%; height:6px; background:#e0e0e0; border-radius:3px; overflow:hidden; margin:20px 0; display:none; }
.progress-fill { height:100%; background: linear-gradient(90deg,#667eea,#764ba2); width:0%; transition: width 0.3s ease; }
@media (max-width:768px) { .container{padding:10px;} .header h1{font-size:2rem;} .card{padding:20px;} }
</style>
</head>
<body>
<div class="container">
    <div class="header">
        <h1>React Code Analyzer</h1>
        <p>Upload or paste your React code to analyze components and generate HTML files</p>
    </div>

    <div class="card">
        <h2>Upload React Code</h2>
        <div class="upload-area" id="uploadArea">
            <p>📁 Drag and drop your React files here or click to browse</p>
            <input type="file" id="fileInput" multiple accept=".js,.jsx,.ts,.tsx" style="display:none;">
        </div>

        <h3 style="margin-top:20px;">Or paste your code:</h3>
        <textarea id="codeInput" placeholder="Paste your React code here..."></textarea>

        <div style="text-align:center; margin-top:20px;">
            <button class="btn" onclick="analyzeCode()">🔍 Analyze Code</button>
            <button class="btn" onclick="generateFiles()">📄 Generate HTML Files</button>
            <button class="btn" onclick="downloadAllFiles()">📦 Download All</button>
            <button class="btn" onclick="clearAll()">🗑️ Clear</button>
        </div>

        <div class="progress-bar" id="progressBar">
            <div class="progress-fill" id="progressFill"></div>
        </div>
    </div>

    <div class="card analysis-result" id="analysisResult">
        <h2>Analysis Results</h2>
        <div id="analysisContent"></div>
    </div>

    <div class="card analysis-result" id="generatedFiles">
        <h2>Generated Files</h2>
        <div id="filesContent"></div>
    </div>
</div>

<!-- JSZip CDN -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/jszip/3.11.0/jszip.min.js"></script>

<script>
let reactCode = '';
const uploadArea = document.getElementById('uploadArea');
const fileInput = document.getElementById('fileInput');

uploadArea.addEventListener('click',()=>fileInput.click());
fileInput.addEventListener('change',handleFileUpload);
uploadArea.addEventListener('dragover',e=>{e.preventDefault(); uploadArea.classList.add('dragover');});
uploadArea.addEventListener('dragleave',()=>uploadArea.classList.remove('dragover'));
uploadArea.addEventListener('drop',e=>{e.preventDefault(); uploadArea.classList.remove('dragover'); handleFileUpload({target:{files:e.dataTransfer.files}});});

function handleFileUpload(event){
    const files = Array.from(event.target.files);
    if(!files.length) return;
    const readers = files.map(file=>{
        return new Promise(resolve=>{
            const reader = new FileReader();
            reader.onload = e=>resolve(`// ${file.name}\n${e.target.result}\n\n`);
            reader.readAsText(file);
        });
    });
    Promise.all(readers).then(results=>{
        reactCode = results.join('');
        document.getElementById('codeInput').value = reactCode;
    });
}

function showProgress(){
    const bar = document.getElementById('progressBar');
    const fill = document.getElementById('progressFill');
    bar.style.display = 'block';
    fill.style.width='0%';
    let width=0;
    return new Promise(resolve=>{
        const interval = setInterval(()=>{
            width+=10; fill.style.width=width+'%';
            if(width>=100){ clearInterval(interval); setTimeout(()=>{bar.style.display='none'; fill.style.width='0%'; resolve();},200);}
        },50);
    });
}

function extractComponents(code){
    const regex=/(?:function|const)\s+([A-Z][a-zA-Z0-9]*)|class\s+([A-Z][a-zA-Z0-9]*)/g;
    const components=[]; let match;
    while((match=regex.exec(code))!==null) components.push(match[1]||match[2]);
    return [...new Set(components)];
}

function extractImports(code){
    const regex=/import\s+.*?from\s+['"]([^'"]+)['"]/g;
    const imports=[]; let match;
    while((match=regex.exec(code))!==null) imports.push(match[1]);
    return imports;
}

function extractHooks(code){
    const hooks=code.match(/use[A-Z][a-zA-Z0-9]*/g)||[];
    return [...new Set(hooks)];
}

function displayAnalysis(components,imports,hooks){
    const content=`<div class="component-list">
    <div class="component-item"><h4>📦 Components (${components.length})</h4><ul>${components.map(c=>`<li>${c}</li>`).join('')}</ul></div>
    <div class="component-item"><h4>📥 Imports (${imports.length})</h4><ul>${imports.map(i=>`<li>${i}</li>`).join('')}</ul></div>
    <div class="component-item"><h4>🎣 Hooks (${hooks.length})</h4><ul>${hooks.map(h=>`<li>${h}</li>`).join('')}</ul></div>
    </div>`;
    document.getElementById('analysisContent').innerHTML=content;
    document.getElementById('analysisResult').style.display='block';
}

async function analyzeCode(){
    const code=document.getElementById('codeInput').value||reactCode;
    if(!code.trim()) return alert('Please provide React code to analyze');
    await showProgress();
    displayAnalysis(extractComponents(code),extractImports(code),extractHooks(code));
}

// Generate HTML from JSX
function generateHTMLFromJSX(code){
    const regex=/(?:function|const)\s+([A-Z][a-zA-Z0-9]*)\s*(?:=\s*\(.*\)\s*=>|\([^)]*\)\s*=>|)\s*{([\s\S]*?)return\s*\(([\s\S]*?)\);/g;
    let match,html='';
    while((match=regex.exec(code))!==null){
        const name=match[1];
        const jsx=match[3].trim()
            .replace(/className=/g,'class=')
            .replace(/\{([^}]+)\}/g,'$1');
        html+=`<div class="component"><h2>${name}</h2>${jsx}</div>\n`;
    }
    if(!html) html=`<div class="app"><h1>Generated from React Code</h1><p>No components detected</p></div>`;
    return `<!DOCTYPE html><html lang="en"><head><meta charset="UTF-8"><meta name="viewport" content="width=device-width, initial-scale=1.0"><title>Generated React App</title><link rel="stylesheet" href="styles.css"></head><body><div id="root">${html}</div><script src="script.js"></script></body></html>`;
}

function generateCSS(){return `.app{max-width:1200px;margin:0 auto;padding:20px;font-family:Arial,sans-serif}.component{background:#f5f5f5;padding:20px;margin:10px 0;border-radius:8px;border:1px solid #ddd}.btn{background:#007bff;color:white;border:none;padding:10px 20px;border-radius:4px;cursor:pointer}.btn:hover{background:#0056b3}`;}

function generateJS(){return `document.addEventListener('DOMContentLoaded',function(){console.log('Generated app loaded');const buttons=document.querySelectorAll('.btn');buttons.forEach(btn=>btn.addEventListener('click',()=>console.log('Button clicked:',btn.textContent)));});`;}

async function generateFiles(){
    const code=document.getElementById('codeInput').value||reactCode;
    if(!code.trim()) return alert('Please provide React code first');
    await showProgress();
    const html=generateHTMLFromJSX(code),css=generateCSS(),js=generateJS();
    displayGeneratedFiles(html,css,js);
}

function displayGeneratedFiles(html,css,js){
    const content=`<div style="display:grid;gap:20px;">
    <div><h3>📄 index.html</h3><textarea readonly style="height:150px;">${html}</textarea><button class="btn" onclick="downloadFile('index.html',html)">Download</button></div>
    <div><h3>🎨 styles.css</h3><textarea readonly style="height:150px;">${css}</textarea><button class="btn" onclick="downloadFile('styles.css',css)">Download</button></div>
    <div><h3>⚡ script.js</h3><textarea readonly style="height:150px;">${js}</textarea><button class="btn" onclick="downloadFile('script.js',js)">Download</button></div>
    </div>`;
    document.getElementById('filesContent').innerHTML=content;
    document.getElementById('generatedFiles').style.display='block';
}

function downloadFile(filename,content){
    const blob=new Blob([content],{type:'text/plain'});
    const url=URL.createObjectURL(blob);
    const a=document.createElement('a');
    a.href=url; a.download=filename; a.click();
    URL.revokeObjectURL(url);
}

// Download all files as ZIP
function downloadAllFiles(){
    const html=generateHTMLFromJSX(document.getElementById('codeInput').value||reactCode);
    const css=generateCSS();
    const js=generateJS();
    const zip=new JSZip();
    zip.file("index.html",html);
    zip.file("styles.css",css);
    zip.file("script.js",js);
    zip.generateAsync({type:"blob"}).then(content=>{
        const url=URL.createObjectURL(content);
        const a=document.createElement("a");
        a.href=url; a.download="ReactApp.zip"; a.click();
        URL.revokeObjectURL(url);
    });
}

function clearAll(){
    document.getElementById('codeInput').value='';
    document.getElementById('analysisResult').style.display='none';
    document.getElementById('generatedFiles').style.display='none';
    reactCode='';
}
</script>
</body>
</html>
