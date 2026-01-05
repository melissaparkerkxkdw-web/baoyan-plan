[Uploading index.html…]()
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>好保研 Unipath - 智能保研规划系统</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Lucide Icons -->
    <script src="https://unpkg.com/lucide@latest"></script>
    <!-- PDF Generation Library -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/html2pdf.js/0.10.1/html2pdf.bundle.min.js"></script>
    <!-- Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        unipath: {
                            50: '#f3f1f8',
                            100: '#e5e0f0',
                            200: '#d0c3e3',
                            300: '#b39cd0',
                            400: '#9470b9',
                            500: '#7b4fa3', 
                            600: '#643a85',
                            700: '#532f6d',
                            800: '#46285a',
                            900: '#3b234a',
                        }
                    },
                    fontFamily: {
                        sans: ['Inter', 'system-ui', 'sans-serif'],
                    },
                    animation: {
                        'fade-in-up': 'fadeInUp 0.5s ease-out forwards',
                        'pulse-slow': 'pulse 3s cubic-bezier(0.4, 0, 0.6, 1) infinite',
                    },
                    keyframes: {
                        fadeInUp: {
                            '0%': { opacity: '0', transform: 'translateY(10px)' },
                            '100%': { opacity: '1', transform: 'translateY(0)' },
                        }
                    }
                }
            }
        }
    </script>
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f8fafc;
        }
        .glass-nav {
            background: rgba(255, 255, 255, 0.8);
            backdrop-filter: blur(12px);
            -webkit-backdrop-filter: blur(12px);
        }
        .pdf-page-break {
            page-break-before: always;
        }
        /* Chart Styles */
        .progress-circle {
            width: 120px;
            height: 120px;
            border-radius: 50%;
            background: conic-gradient(#7b4fa3 var(--percent), #e2e8f0 0);
            display: flex;
            align-items: center;
            justify-content: center;
            position: relative;
        }
        .progress-circle::before {
            content: "";
            width: 100px;
            height: 100px;
            background: white;
            border-radius: 50%;
            position: absolute;
        }
        .bar-segment {
            transition: width 1s ease-in-out;
        }
    </style>
<script type="importmap">
{
  "imports": {
    "react": "https://esm.sh/react@^19.2.3",
    "react-dom/": "https://esm.sh/react-dom@^19.2.3/",
    "react/": "https://esm.sh/react@^19.2.3/",
    "jszip": "https://esm.sh/jszip@^3.10.1",
    "lucide-react": "https://esm.sh/lucide-react@^0.562.0",
    "pptxgenjs": "https://esm.sh/pptxgenjs@^4.0.1"
  }
}
</script>
<link rel="stylesheet" href="/index.css">
</head>
<body class="min-h-screen flex flex-col text-slate-800 bg-gradient-to-br from-indigo-50 via-purple-50 to-pink-50 selection:bg-unipath-200">
    <div id="root"></div>
<script type="module" src="/index.tsx"></script>
</body>
</html>
