    body {
        font-family: 'Segoe UI', 'Inter', system-ui, -apple-system, sans-serif;
        background: linear-gradient(135deg, #fbc2eb 0%, #a6c1ee 100%);
        min-height: 100vh;
        padding: 20px;
    }

    @keyframes fadeIn {
        from { opacity: 0; transform: translateY(10px); }
        to { opacity: 1; transform: translateY(0); }
    }

    .slide-container {
        max-width: 1000px;
        margin: 0 auto;
        background: white;
        border-radius: 32px;
        box-shadow: 0 25px 50px -12px rgba(0, 0, 0, 0.25);
        overflow: hidden;
    }

    /* Transisi halus antar slide */
    .slide-inner {
        padding: 32px 36px;
        transition: opacity 0.28s cubic-bezier(0.2, 0.9, 0.4, 1.1);
        opacity: 1;
        will-change: opacity;
    }

    .slide-inner.fade-out {
        opacity: 0;
    }

    .cover {
        text-align: center;
        background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
        color: white;
        border-radius: 24px;
        padding: 40px 24px;
        margin-bottom: 16px;
    }

    .cover h1 {
        font-size: 2.5rem;
        margin-bottom: 12px;
    }

    .cover h2 {
        font-size: 1.6rem;
        opacity: 0.95;
    }

    .content-block {
        background: #fef2f6;
        border-radius: 20px;
        padding: 20px 26px;
        margin: 16px 0;
        border-left: 5px solid #ec489a;
        transition: all 0.2s;
        line-height: 1.6;
        color: #1e293b;
        font-size: 1rem;
    }

    .content-block.math-block {
        background: #fce7f3;
        border-left-color: #f472b6;
        font-family: 'Courier New', 'SF Mono', monospace;
        overflow-x: auto;
        font-size: 1.05rem;
    }

    .content-block.example {
        background: #fff0f5;
        border-left-color: #f59e0b;
    }

    h3 {
        font-size: 1.6rem;
        color: #be185d;
        margin-bottom: 16px;
        margin-top: 8px;
    }

    h4 {
        font-size: 1.3rem;
        color: #db2777;
        margin-bottom: 12px;
    }

    .badge {
        display: inline-block;
        background: #ec489a;
        color: white;
        padding: 4px 12px;
        border-radius: 20px;
        font-size: 0.75rem;
        font-weight: 600;
        margin-right: 8px;
    }

    .anggota-grid {
        display: flex;
        flex-wrap: wrap;
        gap: 10px;
        margin: 16px 0;
    }

    .anggota-card {
        background: white;
        border: 1px solid #fbcfe8;
        border-radius: 40px;
        padding: 8px 18px;
        font-size: 0.85rem;
        font-weight: 500;
        box-shadow: 0 1px 3px rgba(0,0,0,0.05);
        color: #be185d;
    }

    .nav-buttons {
        display: flex;
        justify-content: center;
        gap: 20px;
        margin: 24px auto 16px;
    }

    button {
        padding: 12px 28px;
        border-radius: 60px;
        border: none;
        font-weight: 600;
        font-size: 1rem;
        cursor: pointer;
        transition: all 0.2s ease;
    }

    .btn-prev {
        background: #9ca3af;
        color: white;
    }

    .btn-prev:hover:not(:disabled) {
        background: #6b7280;
        transform: translateX(-2px);
    }

    .btn-next {
        background: #db2777;
        color: white;
        box-shadow: 0 4px 12px rgba(219, 39, 119, 0.3);
    }

    .btn-next:hover:not(:disabled) {
        background: #be185d;
        transform: translateX(2px);
    }

    button:disabled {
        opacity: 0.5;
        cursor: not-allowed;
    }

    .slide-indicator {
        text-align: center;
        font-size: 0.85rem;
        color: #9ca3af;
        background: rgba(0,0,0,0.05);
        display: inline-block;
        padding: 6px 16px;
        border-radius: 40px;
    }

    .indicator-wrapper {
        text-align: center;
        margin-top: 8px;
    }

    .mcq-option, .tf-btn {
        background: white;
        border: 2px solid #fbcfe8;
        padding: 10px 20px;
        margin: 6px 8px 6px 0;
        display: inline-block;
        border-radius: 40px;
        font-weight: 500;
        cursor: pointer;
        transition: all 0.15s;
        color: #831843;
    }

    .mcq-option:hover, .tf-btn:hover {
        background: #fce7f3;
        border-color: #ec489a;
        transform: scale(1.02);
    }

    .mcq-option.selected {
        border-color: #db2777;
        background: #fce7f3;
    }

    .correct {
        background: #bbf7d0 !important;
        border-color: #16a34a !important;
        color: #166534 !important;
    }

    .incorrect {
        background: #fecaca !important;
        border-color: #dc2626 !important;
        color: #991b1b !important;
    }

    .feedback-msg {
        margin-top: 20px;
        padding: 12px 20px;
        border-radius: 28px;
        font-weight: 500;
    }

    .feedback-msg.correct {
        background: #dcfce7;
        color: #166534;
    }

    .feedback-msg.incorrect {
        background: #fee2e2;
        color: #991b1b;
    }

    .answer-input {
        width: 100%;
        padding: 14px 18px;
        border-radius: 60px;
        border: 2px solid #fbcfe8;
        font-size: 1rem;
        margin: 12px 0;
        transition: 0.2s;
    }

    .answer-input:focus {
        outline: none;
        border-color: #ec489a;
    }

    .check-btn {
        background: #ec489a;
        color: white;
        padding: 10px 28px;
        border-radius: 40px;
    }

    .check-btn:hover {
        background: #db2777;
    }

    hr {
        margin: 20px 0;
        border: none;
        border-top: 2px dashed #fbcfe8;
    }

    /* Animasi getar untuk interaksi belum dijawab */
    @keyframes shake {
        0% { transform: translateX(0); }
        25% { transform: translateX(-4px); }
        75% { transform: translateX(4px); }
        100% { transform: translateX(0); }
    }
    .interactive-area {
        animation: shake 0.2s ease-in-out 0s 1;
    }

    @media (max-width: 700px) {
        .slide-inner { padding: 20px; }
        .content-block { padding: 14px 18px; }
        h3 { font-size: 1.3rem; }
        .mcq-option, .tf-btn { padding: 8px 14px; font-size: 0.85rem; }
    }
</style>
<script>
    window.MathJax = {
        tex: {
            inlineMath: [['\\(', '\\)']],
            displayMath: [['\\[', '\\]']]
        },
        startup: { typeset: false }
    };
</script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-chtml.js"></script>
