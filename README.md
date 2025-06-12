<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>XL-Factor - Excel Conversion Tools</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <style>
        :root {
            --primary: #4a6bff;
            --secondary: #00c6ff;
            --dark: #2d3748;
            --light: #f7fafc;
            --success: #48bb78;
            --warning: #ed8936;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Poppins', sans-serif;
            background-color: #f5f7fa;
            color: var(--dark);
            line-height: 1.6;
        }
        
        .readme-container {
            max-width: 900px;
            margin: 2rem auto;
            padding: 2rem;
            background: white;
            border-radius: 12px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
        }
        
        .header {
            text-align: center;
            margin-bottom: 2rem;
            position: relative;
        }
        
        .header h1 {
            font-size: 2.5rem;
            color: var(--primary);
            margin-bottom: 0.5rem;
            background: linear-gradient(to right, var(--primary), var(--secondary));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        
        .header p {
            font-size: 1.1rem;
            color: #718096;
        }
        
        .domain-badge {
            display: inline-block;
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            color: white;
            padding: 0.5rem 1rem;
            border-radius: 50px;
            margin-top: 1rem;
            font-weight: 600;
            box-shadow: 0 4px 15px rgba(74, 107, 255, 0.3);
        }
        
        .divider {
            height: 3px;
            background: linear-gradient(to right, transparent, var(--primary), transparent);
            margin: 1.5rem 0;
            border: none;
        }
        
        .section {
            margin-bottom: 2rem;
        }
        
        .section-title {
            font-size: 1.5rem;
            color: var(--primary);
            margin-bottom: 1rem;
            display: flex;
            align-items: center;
        }
        
        .section-title i {
            margin-right: 0.5rem;
        }
        
        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 1.5rem;
            margin-top: 1.5rem;
        }
        
        .feature-card {
            background: white;
            border-radius: 8px;
            padding: 1.5rem;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s, box-shadow 0.3s;
            border: 1px solid #e2e8f0;
        }
        
        .feature-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
        }
        
        .feature-icon {
            font-size: 2rem;
            margin-bottom: 1rem;
            color: var(--primary);
        }
        
        .feature-card h3 {
            font-size: 1.1rem;
            margin-bottom: 0.5rem;
            color: var(--dark);
        }
        
        .feature-card p {
            font-size: 0.9rem;
            color: #718096;
        }
        
        .conversion-chart {
            margin-top: 2rem;
            height: 300px;
        }
        
        .badges {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
            margin-top: 1rem;
        }
        
        .badge {
            display: inline-block;
            padding: 0.3rem 0.8rem;
            border-radius: 50px;
            font-size: 0.8rem;
            font-weight: 600;
        }
        
        .badge-primary {
            background-color: rgba(74, 107, 255, 0.1);
            color: var(--primary);
        }
        
        .badge-success {
            background-color: rgba(72, 187, 120, 0.1);
            color: var(--success);
        }
        
        .badge-warning {
            background-color: rgba(237, 137, 54, 0.1);
            color: var(--warning);
        }
        
        .cta-button {
            display: inline-block;
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            color: white;
            padding: 0.8rem 1.5rem;
            border-radius: 8px;
            text-decoration: none;
            font-weight: 600;
            margin-top: 1rem;
            transition: transform 0.3s, box-shadow 0.3s;
            box-shadow: 0 4px 15px rgba(74, 107, 255, 0.3);
        }
        
        .cta-button:hover {
            transform: translateY(-2px);
            box-shadow: 0 6px 20px rgba(74, 107, 255, 0.4);
            color: white;
        }
        
        .footer {
            text-align: center;
            margin-top: 3rem;
            color: #718096;
            font-size: 0.9rem;
        }
        
        @media (max-width: 768px) {
            .readme-container {
                padding: 1.5rem;
            }
            
            .header h1 {
                font-size: 2rem;
            }
            
            .features-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <div class="readme-container">
        <div class="header">
            <h1>XL-Factor</h1>
            <p>Powerful Excel Conversion and Processing Tools - Absolutely Free!</p>
            <div class="domain-badge">
                <i class="fas fa-globe"></i> www.xl-factor.com
            </div>
        </div>
        
        <hr class="divider">
        
        <div class="section">
            <h2 class="section-title"><i class="fas fa-info-circle"></i> About XL-Factor</h2>
            <p>XL-Factor is a comprehensive online platform that provides a suite of tools for converting and processing Excel files in various formats. Our mission is to simplify data manipulation tasks for professionals, students, and anyone who works with spreadsheets.</p>
            
            <div class="badges">
                <span class="badge badge-success"><i class="fas fa-lock-open"></i> 100% Free</span>
                <span class="badge badge-primary"><i class="fas fa-bolt"></i> Fast Processing</span>
                <span class="badge badge-warning"><i class="fas fa-shield-alt"></i> Secure</span>
                <span class="badge badge-primary"><i class="fas fa-cloud"></i> No Installation</span>
            </div>
            
            <a href="https://www.xl-factor.com" class="cta-button" target="_blank">
                <i class="fas fa-external-link-alt"></i> Visit Website
            </a>
        </div>
        
        <hr class="divider">
        
        <div class="section">
            <h2 class="section-title"><i class="fas fa-exchange-alt"></i> Conversion Tools</h2>
            <p>Seamlessly convert between Excel and various other formats with our high-quality conversion tools.</p>
            
            <div class="features-grid">
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-file-excel"></i> <i class="fas fa-arrow-right"></i> <i class="fas fa-file-csv"></i>
                    </div>
                    <h3>Excel to CSV</h3>
                    <p>Convert your Excel spreadsheets to CSV format while preserving all your data structure and formatting.</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-file-excel"></i> <i class="fas fa-arrow-right"></i> <i class="fas fa-file-pdf"></i>
                    </div>
                    <h3>Excel to PDF</h3>
                    <p>Transform your Excel files into professional PDF documents perfect for sharing and printing.</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-file-excel"></i> <i class="fas fa-arrow-right"></i> <i class="fas fa-file-code"></i>
                    </div>
                    <h3>Excel to JSON</h3>
                    <p>Convert Excel data to JSON format for easy integration with web applications and APIs.</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-file-csv"></i> <i class="fas fa-arrow-right"></i> <i class="fas fa-file-excel"></i>
                    </div>
                    <h3>CSV to Excel</h3>
                    <p>Convert CSV files back to Excel format with proper column formatting and data types.</p>
                </div>
            </div>
            
            <div class="conversion-chart">
                <canvas id="conversionChart"></canvas>
            </div>
        </div>
        
        <hr class="divider">
        
        <div class="section">
            <h2 class="section-title"><i class="fas fa-tools"></i> Processing Tools</h2>
            <p>Powerful tools to manipulate and process your Excel files without any complex software.</p>
            
            <div class="features-grid">
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-object-group"></i>
                    </div>
                    <h3>Merge Excel Files</h3>
                    <p>Combine multiple Excel files into a single workbook while maintaining all sheets and formatting.</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-layer-group"></i>
                    </div>
                    <h3>Merge Sheets</h3>
                    <p>Merge multiple sheets from different workbooks into one comprehensive sheet.</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-cut"></i>
                    </div>
                    <h3>Split Sheet</h3>
                    <p>Divide a large Excel sheet into multiple smaller sheets based on your criteria.</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-search"></i>
                    </div>
                    <h3>V Lookup</h3>
                    <p>Perform vertical lookups between sheets to find and match data effortlessly.</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-image"></i> <i class="fas fa-search"></i>
                    </div>
                    <h3>Image V Lookup</h3>
                    <p>Our unique tool that allows you to perform lookups using images as references.</p>
                </div>
            </div>
        </div>
        
        <hr class="divider">
        
        <div class="section">
            <h2 class="section-title"><i class="fas fa-star"></i> Why Choose XL-Factor?</h2>
            <div class="features-grid">
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-dollar-sign"></i>
                    </div>
                    <h3>Completely Free</h3>
                    <p>All our tools are 100% free with no hidden charges or premium tiers.</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-tachometer-alt"></i>
                    </div>
                    <h3>Lightning Fast</h3>
                    <p>Optimized algorithms ensure your files are processed in seconds.</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-user-shield"></i>
                    </div>
                    <h3>Privacy Focused</h3>
                    <p>Your files are processed in your browser and never uploaded to our servers.</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-desktop"></i>
                    </div>
                    <h3>No Installation</h3>
                    <p>Access all tools directly from your browser without any downloads.</p>
                </div>
            </div>
        </div>
        
        <div class="footer">
            <p>© 2023 XL-Factor | www.xl-factor.com | All Rights Reserved</p>
            <p>Made with <i class="fas fa-heart" style="color: #ff4757;"></i> for Excel users worldwide</p>
        </div>
    </div>

    <script>
        // Chart for conversion statistics
        document.addEventListener('DOMContentLoaded', function() {
            const ctx = document.getElementById('conversionChart').getContext('2d');
            const chart = new Chart(ctx, {
                type: 'bar',
                data: {
                    labels: ['Excel to CSV', 'Excel to PDF', 'Excel to JSON', 'CSV to Excel'],
                    datasets: [{
                        label: 'Conversions Per Day (Thousands)',
                        data: [45, 32, 28, 38],
                        backgroundColor: [
                            'rgba(74, 107, 255, 0.7)',
                            'rgba(255, 99, 132, 0.7)',
                            'rgba(54, 162, 235, 0.7)',
                            'rgba(75, 192, 192, 0.7)'
                        ],
                        borderColor: [
                            'rgba(74, 107, 255, 1)',
                            'rgba(255, 99, 132, 1)',
                            'rgba(54, 162, 235, 1)',
                            'rgba(75, 192, 192, 1)'
                        ],
                        borderWidth: 1
                    }]
                },
                options: {
                    responsive: true,
                    plugins: {
                        legend: {
                            position: 'top',
                        },
                        title: {
                            display: true,
                            text: 'Popular Conversion Tools',
                            font: {
                                size: 16
                            }
                        }
                    },
                    scales: {
                        y: {
                            beginAtZero: true,
                            title: {
                                display: true,
                                text: 'Conversions (Thousands)'
                            }
                        }
                    }
                }
            });
            
            // Add animation to feature cards on scroll
            const featureCards = document.querySelectorAll('.feature-card');
            
            const observer = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.style.opacity = 1;
                        entry.target.style.transform = 'translateY(0)';
                    }
                });
            }, { threshold: 0.1 });
            
            featureCards.forEach(card => {
                card.style.opacity = 0;
                card.style.transform = 'translateY(20px)';
                card.style.transition = 'opacity 0.5s ease, transform 0.5s ease';
                observer.observe(card);
            });
        });
    </script>
</body>
</html>
