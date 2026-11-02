/* ==========================================
   SM POULTRY - MASTER STYLESHEET
   ========================================== */

/* --- CSS Variables & Color Palette --- */
:root {
    --primary: #2e6f40;
    --primary-dark: #22532f;
    --secondary: #e6a100;
    --secondary-hover: #c78b00;
    --dark: #222222;
    --light: #f4f7f4;
    --white: #ffffff;
    --gray-light: #e0e0e0;
    --gray-text: #555555;
    --shadow: 0 4px 15px rgba(0, 0, 0, 0.08);
    --shadow-hover: 0 8px 25px rgba(0, 0, 0, 0.12);
    --transition: all 0.3s ease;
    --whatsapp-color: #25D366;
    --whatsapp-hover: #1ebd59;
}

/* --- Base & Reset Styles --- */
html {
    scroll-behavior: smooth;
}

* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

body {
    background-color: var(--light);
    color: var(--dark);
    line-height: 1.6;
    display: flex;
    flex-direction: column;
    min-height: 100vh;
}

/* --- Navigation & Header --- */
header {
    background-color: var(--primary);
    color: var(--white);
    padding: 1rem 5%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    position: sticky;
    top: 0;
    z-index: 1000;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.15);
}

.logo {
    font-size: 1.6rem;
    font-weight: 700;
    color: var(--secondary);
    display: flex;
    align-items: center;
    gap: 10px;
}

nav {
    display: flex;
    align-items: center;
    gap: 1.5rem;
}

nav a {
    color: var(--white);
    text-decoration: none;
    font-weight: 500;
    transition: var(--transition);
    position: relative;
    padding: 0.2rem 0;
}

nav a::after {
    content: '';
    position: absolute;
    width: 0;
    height: 2px;
    bottom: 0;
    left: 0;
    background-color: var(--secondary);
    transition: var(--transition);
}

nav a:hover::after, 
nav a.active::after {
    width: 100%;
}

nav a:hover, 
nav a.active {
    color: var(--secondary);
}

.menu-toggle {
    display: none;
    font-size: 1.5rem;
    color: var(--white);
    cursor: pointer;
}

/* --- Reading Progress Bar (Guides Page) --- */
.progress-bar {
    position: fixed;
    top: 60px;
    left: 0;
    height: 4px;
    background: var(--secondary);
    width: 0%;
    z-index: 999;
    transition: width 0.1s ease;
}

/* --- Page Banners --- */
.page-banner {
    background: linear-gradient(rgba(46, 111, 64, 0.9), rgba(34, 83, 47, 0.9)), 
                url('https://images.unsplash.com/photo-1548550023-2bdb3c5beed7?auto=format&fit=crop&w=1200&q=80') center/cover;
    color: var(--white);
    text-align: center;
    padding: 4rem 1rem;
}

.page-banner h1 {
    font-size: 2.5rem;
    margin-bottom: 0.5rem;
    animation: fadeInDown 0.8s ease;
}

.page-banner p {
    font-size: 1.15rem;
    opacity: 0.9;
    animation: fadeInUp 0.8s ease;
}

/* --- Container Layouts --- */
.container {
    max-width: 1100px;
    margin: 3rem auto;
    padding: 0 1.5rem;
    flex: 1;
}

.container-narrow {
    max-width: 900px;
    margin: 3rem auto;
    padding: 0 1.5rem;
    flex: 1;
}

/* --- Controls Section (Filter & Live Search Bar) --- */
.controls-container, .search-container {
    max-width: 1100px;
    margin: 2rem auto 0 auto;
    padding: 0 1.5rem;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: center;
    gap: 1.5rem;
}

.search-box {
    position: relative;
    flex: 1;
    min-width: 250px;
}

.search-box input {
    width: 100%;
    padding: 0.85rem 1rem 0.85rem 2.8rem;
    border: 2px solid var(--gray-light);
    border-radius: 30px;
    font-size: 0.95rem;
    outline: none;
    transition: var(--transition);
    box-shadow: var(--shadow);
}

.search-box input:focus {
    border-color: var(--primary);
}

.search-box i {
    position: absolute;
    left: 1.2rem;
    top: 50%;
    transform: translateY(-50%);
    color: #888;
}

.filter-buttons {
    display: flex;
    flex-wrap: wrap;
    gap: 0.5rem;
}

.filter-btn {
    background: var(--white);
    border: 1px solid #ddd;
    padding: 0.5rem 1.2rem;
    border-radius: 20px;
    font-size: 0.9rem;
    font-weight: 600;
    cursor: pointer;
    color: var(--dark);
    transition: var(--transition);
}

.filter-btn:hover,
.filter-btn.active {
    background-color: var(--primary);
    color: var(--white);
    border-color: var(--primary);
}

/* --- Products & Catalog Cards --- */
.grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 2rem;
}

.product-card {
    background: var(--white);
    border-radius: 12px;
    overflow: hidden;
    box-shadow: var(--shadow);
    display: flex;
    flex-direction: column;
    transition: var(--transition);
    opacity: 0;
    transform: translateY(20px);
}

.product-card.reveal {
    opacity: 1;
    transform: translateY(0);
}

.product-card:hover {
    transform: translateY(-6px);
    box-shadow: var(--shadow-hover);
}

.image-container {
    position: relative;
    width: 100%;
    height: 220px;
    overflow: hidden;
    background-color: #eee;
}

.product-image {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: var(--transition);
}

.product-card:hover .product-image {
    transform: scale(1.05);
}

.badge {
    position: absolute;
    top: 12px;
    left: 12px;
    background-color: var(--secondary);
    color: var(--dark);
    padding: 0.3rem 0.75rem;
    font-size: 0.75rem;
    font-weight: bold;
    border-radius: 20px;
    text-transform: uppercase;
    box-shadow: 0 2px 5px rgba(0,0,0,0.2);
}

.product-details {
    padding: 1.5rem;
    display: flex;
    flex-direction: column;
    flex: 1;
}

.product-details h3 {
    color: var(--primary);
    margin-bottom: 0.5rem;
    font-size: 1.25rem;
}

.product-details p {
    color: var(--gray-text);
    font-size: 0.95rem;
    margin-bottom: 1.2rem;
    flex: 1;
}

.card-actions {
    display: flex;
    gap: 0.5rem;
}

.btn-inquire {
    flex: 1;
    background-color: var(--primary);
    color: var(--white);
    border: none;
    padding: 0.65rem;
    border-radius: 6px;
    font-weight: bold;
    cursor: pointer;
    transition: var(--transition);
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 6px;
    font-size: 0.9rem;
    text-decoration: none;
}

.btn-inquire:hover {
    background-color: var(--primary-dark);
}

.btn-whatsapp-icon {
    background-color: var(--whatsapp-color);
    color: var(--white);
    border: none;
    padding: 0.65rem 0.8rem;
    border-radius: 6px;
    cursor: pointer;
    transition: var(--transition);
    display: flex;
    align-items: center;
    justify-content: center;
    text-decoration: none;
}

.btn-whatsapp-icon:hover {
    background-color: var(--whatsapp-hover);
}

/* --- Farming Guides Accordion --- */
.guide-post {
    background: var(--white);
    border-radius: 12px;
    box-shadow: var(--shadow);
    margin-bottom: 1.5rem;
    overflow: hidden;
    transition: var(--transition);
    opacity: 0;
    transform: translateY(20px);
}

.guide-post.reveal {
    opacity: 1;
    transform: translateY(0);
}

.guide-header {
    padding: 1.5rem;
    background: var(--white);
    cursor: pointer;
    display: flex;
    justify-content: space-between;
    align-items: center;
    user-select: none;
    transition: var(--transition);
}

.guide-header:hover {
    background-color: #f8faf8;
}

.guide-header h2 {
    color: var(--primary);
    font-size: 1.25rem;
    display: flex;
    align-items: center;
    gap: 12px;
}

.guide-header .toggle-icon {
    color: var(--primary);
    font-size: 1.2rem;
    transition: transform 0.3s ease;
}

.guide-post.open .toggle-icon {
    transform: rotate(180deg);
}

.guide-content {
    max-height: 0;
    overflow: hidden;
    transition: max-height 0.4s ease, padding 0.4s ease;
    padding: 0 1.5rem;
    background: var(--white);
    border-top: 1px solid transparent;
}

.guide-post.open .guide-content {
    max-height: 500px;
    padding: 1rem 1.5rem 1.5rem 1.5rem;
    border-top: 1px solid #eee;
}

.guide-content p {
    color: #444;
    margin-bottom: 0.8rem;
}

.guide-content ul {
    margin-left: 1.2rem;
    display: flex;
    flex-direction: column;
    gap: 0.6rem;
}

.guide-content ul li {
    color: var(--gray-text);
}

/* --- Contact & Inquiry Page Styles --- */
.contact-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
    gap: 2rem;
}

.info-box, .form-box {
    background: var(--white);
    padding: 2.5rem;
    border-radius: 12px;
    box-shadow: var(--shadow);
    opacity: 0;
    transform: translateY(30px);
    transition: var(--transition);
}

.info-box.reveal, .form-box.reveal, .map-section.reveal {
    opacity: 1;
    transform: translateY(0);
}

.info-box h2, .form-box h2 {
    color: var(--primary);
    margin-bottom: 1.5rem;
    display: flex;
    align-items: center;
    gap: 10px;
    border-bottom: 2px solid var(--light);
    padding-bottom: 0.5rem;
}

.contact-list {
    list-style: none;
    display: flex;
    flex-direction: column;
    gap: 1.25rem;
}

.contact-item {
    display: flex;
    align-items: flex-start;
    gap: 1rem;
}

.contact-icon {
    background: var(--light);
    color: var(--primary);
    width: 42px;
    height: 42px;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 1.2rem;
    flex-shrink: 0;
}

.contact-text strong {
    display: block;
    color: var(--primary-dark);
    font-size: 0.95rem;
}

.contact-text p, .contact-text a {
    color: var(--gray-text);
    font-size: 0.95rem;
    text-decoration: none;
}

.contact-text a:hover {
    color: var(--primary);
    text-decoration: underline;
}

.whatsapp-btn {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 10px;
    background-color: var(--whatsapp-color);
    color: var(--white);
    text-decoration: none;
    padding: 0.85rem;
    border-radius: 8px;
    font-weight: bold;
    margin-top: 1.5rem;
    transition: var(--transition);
    box-shadow: 0 4px 10px rgba(37, 211, 102, 0.2);
}

.whatsapp-btn:hover {
    background-color: var(--whatsapp-hover);
    transform: translateY(-2px);
}

/* --- Forms & Inputs --- */
.form-group {
    margin-bottom: 1.2rem;
}

.form-group label {
    display: block;
    margin-bottom: 0.4rem;
    font-weight: 600;
    color: var(--dark);
    font-size: 0.9rem;
}

.form-group input, 
.form-group select, 
.form-group textarea {
    width: 100%;
    padding: 0.8rem 1rem;
    border: 1px solid #ccc;
    border-radius: 6px;
    font-size: 0.95rem;
    transition: var(--transition);
    outline: none;
}

.form-group input:focus, 
.form-group select:focus, 
.form-group textarea:focus {
    border-color: var(--primary);
    box-shadow: 0 0 0 3px rgba(46, 111, 64, 0.15);
}

.btn-submit {
    background-color: var(--primary);
    color: var(--white);
    border: none;
    padding: 0.85rem 1.5rem;
    font-size: 1rem;
    font-weight: bold;
    border-radius: 6px;
    cursor: pointer;
    width: 100%;
    transition: var(--transition);
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 8px;
}

.btn-submit:hover {
    background-color: var(--primary-dark);
    transform: translateY(-2px);
}

.form-status {
    margin-top: 1rem;
    padding: 0.75rem;
    border-radius: 6px;
    font-size: 0.9rem;
    display: none;
    text-align: center;
}

.form-status.success {
    display: block;
    background-color: #d4edda;
    color: #155724;
    border: 1px solid #c3e6cb;
}

/* --- Map Component --- */
.map-section {
    max-width: 1050px;
    margin: 0 auto 3rem auto;
    padding: 0 1.5rem;
    opacity: 0;
    transform: translateY(30px);
    transition: var(--transition);
}

.map-container {
    background: var(--white);
    padding: 2rem;
    border-radius: 12px;
    box-shadow: var(--shadow);
}

.map-container h2 {
    color: var(--primary);
    margin-bottom: 0.5rem;
    display: flex;
    align-items: center;
    gap: 10px;
}

.map-frame {
    width: 100%;
    height: 380px;
    border: none;
    border-radius: 8px;
    margin-top: 1rem;
}

/* --- Modal Dialog --- */
.modal {
    display: none;
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.6);
    z-index: 2000;
    justify-content: center;
    align-items: center;
    padding: 1rem;
}

.modal.active {
    display: flex;
    animation: fadeIn 0.3s ease;
}

.modal-content {
    background: var(--white);
    padding: 2rem;
    border-radius: 12px;
    width: 100%;
    max-width: 500px;
    position: relative;
    box-shadow: 0 5px 20px rgba(0,0,0,0.2);
}

.modal-close {
    position: absolute;
    top: 15px;
    right: 15px;
    font-size: 1.5rem;
    cursor: pointer;
    color: #888;
    transition: var(--transition);
}

.modal-close:hover {
    color: var(--dark);
}

.no-results {
    text-align: center;
    padding: 3rem 1rem;
    color: #777;
    display: none;
    grid-column: 1 / -1;
}

/* --- Back to Top Button --- */
.back-to-top {
    position: fixed;
    bottom: 20px;
    right: 20px;
    background-color: var(--primary);
    color: var(--white);
    width: 45px;
    height: 45px;
    border-radius: 50%;
    display: flex;
    justify-content: center;
    align-items: center;
    text-decoration: none;
    opacity: 0;
    visibility: hidden;
    transition: var(--transition);
    box-shadow: var(--shadow);
    z-index: 999;
}

.back-to-top.visible {
    opacity: 1;
    visibility: visible;
}

.back-to-top:hover {
    background-color: var(--secondary);
    color: var(--dark);
}

/* --- Footer --- */
footer {
    background-color: var(--primary);
    color: var(--white);
    text-align: center;
    padding: 2rem 1rem;
    margin-top: auto;
}

/* --- Keyframe Animations --- */
@keyframes fadeInDown {
    from { opacity: 0; transform: translateY(-20px); }
    to { opacity: 1; transform: translateY(0); }
}

@keyframes fadeInUp {
    from { opacity: 0; transform: translateY(20px); }
    to { opacity: 1; transform: translateY(0); }
}

@keyframes fadeIn {
    from { opacity: 0; }
    to { opacity: 1; }
}

/* --- Responsive Media Queries --- */
@media (max-width: 768px) {
    .menu-toggle {
        display: block;
    }

    nav {
        display: none;
        flex-direction: column;
        position: absolute;
        top: 100%;
        left: 0;
        width: 100%;
        background-color: var(--primary-dark);
        padding: 1.5rem 0;
        gap: 1rem;
        box-shadow: 0 5px 10px rgba(0,0,0,0.2);
    }

    nav.active {
        display: flex;
    }

    nav a {
        margin: 0;
    }

    .controls-container {
        flex-direction: column;
        align-items: stretch;
    }

    .filter-buttons {
        justify-content: center;
    }

    .guide-header h2 {
        font-size: 1.05rem;
    }
}