<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>index.html - 이미지 스크롤 뷰어</title>

  <!-- Discord / SNS 공유용 메타태그 -->
  <meta property="og:title" content="공유용 이미지 갤러리">
  <meta property="og:description" content="스크롤하면서 볼 수 있는 이미지 모음">
  <meta property="og:type" content="website">

  <style>
    :root{--bg:#0f172a;--panel:#111827;--muted:#94a3b8;--text:#e5e7eb;--accent:#60a5fa;--accent-2:#38bdf8;--border:#1f2937;--ok:#10b981;--warn:#f59e0b}
    *{box-sizing:border-box}
    html,body{height:100%}
    body{margin:0;background:linear-gradient(180deg,var(--bg),#0b1220 60%);color:var(--text);font-family:ui-sans-serif,system-ui,-apple-system,Segoe UI,Roboto,"Noto Sans KR","Apple SD Gothic Neo","Malgun Gothic",Arial,"Apple Color Emoji","Segoe UI Emoji"; display:flex; flex-direction:column;}

    header{position:sticky;top:0;z-index:10;backdrop-filter:blur(8px);background:rgba(15,23,42,0.7);border-bottom:1px solid var(--border); padding:16px;}
    header h1{margin:0;font-weight:800;letter-spacing:-0.02em;}
    .sub{color:var(--muted);font-size:14px; margin-top:4px;}

    .controls{display:flex; justify-content:center; gap:12px; margin:12px 0;}
    .btn{padding:8px 16px; border-radius:8px; border:none; cursor:pointer; font-weight:600; background-color:var(--accent); color:#00111a; transition:0.15s;}
    .btn:hover{opacity:0.85;}

    main.gallery{flex:1; overflow-y:auto; max-width:1100px; margin:0 auto; display:flex; flex-direction:column; gap:16px; padding:16px;}
    .preview{display:block;width:100%;height:auto;background:#000; border-radius:12px;}
  </style>
</head>
<body>
  <header>
    <h1>index.html - 이미지 스크롤 뷰어</h1>
    <div class="sub">HTML 파일을 공유하려면 이 파일(index.html)을 그대로 보내면 됩니다.</div>
    <div class="controls">
      <button class="btn" id="uploadBtn">이미지 업로드</button>
    </div>
  </header>

  <main class="gallery" id="gallery"></main>

  <script>
    const gallery = document.getElementById('gallery');
    const uploadBtn = document.getElementById('uploadBtn');
    let items = [];

    function addImage(file){
      if(!file.type.startsWith('image/')) return;
      const reader = new FileReader();
      reader.onload = ()=>{
        const dataUrl = reader.result;
        const img = document.createElement('img');
        img.src = dataUrl;
        img.className = 'preview';
        gallery.appendChild(img);
        items.push({file,fileName:file.name,dataUrl});
        if(items.length === 1){
          let meta = document.querySelector('meta[property="og:image"]');
          if(!meta){
            meta = document.createElement('meta');
            meta.setAttribute('property','og:image');
            document.head.appendChild(meta);
          }
          meta.setAttribute('content', dataUrl);
          console.log('대표 이미지 og:image URL:', dataUrl);
        }
      };
      reader.readAsDataURL(file);
    }

    uploadBtn.addEventListener('click', ()=>{
      const input = document.createElement('input');
      input.type='file'; input.accept='image/*'; input.multiple=true;
      input.onchange = e=>{Array.from(e.target.files).forEach(addImage);};
      input.click();
    });
  </script>
</body>
</html>
