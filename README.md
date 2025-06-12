<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>XL-Factor - GitHub Readme</title>
    <!-- Tailwind CSS CDN for utility classes -->
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        /*
         * Custom CSS styles to enhance the visual appeal beyond Tailwind's utility classes.
         * This includes custom fonts, shadows, border accents, and hover effects for interactivity.
         */
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap');
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f8f8f8; /* Light gray background for the page */
        }
        .container {
            /* Styles for the main content container, simulating a README card */
            max-width: 960px; /* Standard width for better readability */
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1); /* Soft shadow for depth */
            border-radius: 12px; /* Rounded corners for modern look */
            overflow: hidden; /* Ensures content respects rounded corners */
            border: 1px solid #e0e0e0; /* Subtle border */
        }
        .section-header {
            /* Styling for section titles with a left accent border */
            border-left: 5px solid #2563eb; /* Blue accent border */
            padding-left: 1rem; /* Spacing for the text next to the border */
        }
        .icon-grid i {
            /* Styling for Font Awesome icons in the tech stack section */
            transition: transform 0.2s ease-in-out; /* Smooth hover effect */
        }
        .icon-grid i:hover {
            transform: translateY(-5px); /* Lift effect on hover */
        }
        .tool-card {
            /* Styling for individual tool cards with hover effects */
            transition: transform 0.2s ease-in-out, box-shadow 0.2s ease-in-out; /* Smooth transitions */
        }
        .tool-card:hover {
            transform: translateY(-5px); /* Lift effect on hover */
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.15); /* Enhanced shadow on hover */
        }
        .btn-primary {
            /* Styling for the primary call-to-action button with gradient and hover effect */
            background-image: linear-gradient(to right, #4CAF50 0%, #2e7d32  51%, #4CAF50  100%);
            margin: 10px;
            padding: 15px 45px;
            text-align: center;
            text-transform: uppercase;
            transition: 0.5s; /* Smooth transition for background position */
            background-size: 200% auto; /* Allows the gradient to shift on hover */
            color: white;
            box-shadow: 0 0 20px #eee;
            border-radius: 10px;
            display: inline-block; /* Changed from block to inline-block for better centering */
        }
        .btn-primary:hover {
            background-position: right center; /* Shifts the gradient on hover */
            color: #fff;
            text-decoration: none;
        }

        /* Responsive adjustments for smaller screens */
        @media (max-width: 768px) {
            .container {
                margin: 1rem; /* Add margin on smaller screens */
            }
            .tool-card-grid {
                grid-template-columns: 1fr; /* Stack tool cards vertically on small screens */
            }
        }
    </style>
    <!-- Font Awesome CDN for various icons (e.g., file types, tools) -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css" xintegrity="sha512-Fo3rlrZj/k7ujTnHg4CGR2D7kSs0x0UgO/Y8fX1hXJ2jT8S2s3w9VbFh5B/p5K5S2p1z02e2L0A2l3C/n3X3Q==" crossorigin="anonymous" referrerpolicy="no-referrer" />
    <!-- Chart.js CDN for creating attractive data charts -->
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
</head>
<body class="p-8">
    <div class="container mx-auto bg-white p-8 md:p-12">

        <!-- Header Section: Main title, tagline, and a prominent call to action -->
        <header class="text-center mb-12">
            <h1 class="text-5xl font-extrabold text-gray-800 mb-4">
                XL-Factor
            </h1>
            <p class="text-2xl text-gray-600 mb-6">
                Your Ultimate Excel Conversion & Processing Hub
            </p>
            <p class="text-lg text-gray-700 max-w-2xl mx-auto">
                Free, Fast, and Feature-Rich Tools for All Your Spreadsheet Needs.
                Simplify your data workflows with our powerful online tools.
            </p>
            <a href="https://www.xl-factor.com" target="_blank" class="inline-block mt-8 btn-primary">
                Visit XL-Factor Now!
            </a>
        </header>

        <!-- About Website Section: Provides detailed information about XL-Factor -->
        <section class="mb-12">
            <h2 class="text-3xl font-bold text-gray-800 mb-6 section-header">
                About XL-Factor
            </h2>
            <div class="bg-blue-50 p-6 rounded-lg">
                <p class="text-lg text-gray-700 leading-relaxed mb-4">
                    XL-Factor is a revolutionary online platform dedicated to providing <strong class="text-blue-700">absolutely free</strong> and efficient tools for all your Excel file manipulation needs. Our mission is to empower users with robust functionalities without any cost.
                </p>
                <ul class="list-disc list-inside text-gray-700 space-y-2">
                    <li><strong class="font-semibold">Domain:</strong> <a href="https://www.xl-factor.com" target="_blank" class="text-blue-600 hover:underline">www.xl-factor.com</a></li>
                    <li><strong class="font-semibold">Core Function:</strong> Seamless Excel file conversion and advanced processing.</li>
                    <li><strong class="font-semibold">Cost:</strong> All tools are <span class="text-green-600 font-bold">100% FREE!</span></li>
                </ul>
            </div>
        </section>

        <!-- Key Features Section: Highlights the various free tools offered -->
        <section class="mb-12">
            <h2 class="text-3xl font-bold text-gray-800 mb-6 section-header">
                Our Powerful & Free Tools
            </h2>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6 tool-card-grid">
                <!-- Tool Card: Excel Conversion -->
                <div class="tool-card bg-white p-6 rounded-lg shadow-md border border-gray-200">
                    <h3 class="text-xl font-semibold text-gray-800 mb-3 flex items-center">
                        <i class="fas fa-file-excel text-green-600 mr-3 text-2xl"></i> Excel Conversion
                    </h3>
                    <p class="text-gray-700">
                        Effortlessly convert Excel files to various formats like CSV, PDF, and JSON, and vice versa. Your data, your format.
                    </p>
                </div>
                <!-- Tool Card: Merge Excel -->
                <div class="tool-card bg-white p-6 rounded-lg shadow-md border border-gray-200">
                    <h3 class="text-xl font-semibold text-gray-800 mb-3 flex items-center">
                        <i class="fas fa-layer-group text-purple-600 mr-3 text-2xl"></i> Merge Excel
                    </h3>
                    <p class="text-gray-700">
                        Combine multiple Excel files into a single, unified document quickly and accurately.
                    </p>
                </div>
                <!-- Tool Card: Merge Sheet -->
                <div class="tool-card bg-white p-6 rounded-lg shadow-md border border-gray-200">
                    <h3 class="text-xl font-semibold text-gray-800 mb-3 flex items-center">
                        <i class="fas fa-table text-indigo-600 mr-3 text-2xl"></i> Merge Sheet
                    </h3>
                    <p class="text-gray-700">
                        Consolidate data from different sheets within an Excel workbook into one master sheet.
                    </p>
                </div>
                <!-- Tool Card: Split Sheet -->
                <div class="tool-card bg-white p-6 rounded-lg shadow-md border border-gray-200">
                    <h3 class="text-xl font-semibold text-gray-800 mb-3 flex items-center">
                        <i class="fas fa-cut text-red-600 mr-3 text-2xl"></i> Split Sheet
                    </h3>
                    <p class="text-gray-700">
                        Divide large Excel sheets into smaller, manageable files based on specified criteria.
                    </p>
                </div>
                <!-- Tool Card: V Lookup -->
                <div class="tool-card bg-white p-6 rounded-lg shadow-md border border-gray-200">
                    <h3 class="text-xl font-semibold text-gray-800 mb-3 flex items-center">
                        <i class="fas fa-search text-orange-600 mr-3 text-2xl"></i> V Lookup
                    </h3>
                    <p class="text-gray-700">
                        Perform fast and accurate VLOOKUP operations online without needing Excel software.
                    </p>
                </div>
                <!-- Tool Card: Image V Lookup -->
                <div class="tool-card bg-white p-6 rounded-lg shadow-md border border-gray-200">
                    <h3 class="text-xl font-semibold text-gray-800 mb-3 flex items-center">
                        <i class="fas fa-image text-cyan-600 mr-3 text-2xl"></i> Image V Lookup
                    </h3>
                    <p class="text-gray-700">
                        A unique tool to match data and images, expanding your data processing capabilities.
                    </p>
                </div>
            </div>
        </section>

        <!-- Technology Stack Section: Showcases the underlying technologies using Font Awesome brand icons -->
        <section class="mb-12">
            <h2 class="text-3xl font-bold text-gray-800 mb-6 section-header">
                Built with Modern Technologies
            </h2>
            <p class="text-gray-700 mb-6">
                XL-Factor is powered by a robust and scalable technology stack to ensure performance and reliability.
            </p>
            <div class="flex flex-wrap justify-center items-center gap-8 icon-grid">
                <!-- Icons for different technologies/languages. Assuming standard web development stack. -->
                <div class="text-center">
                    <i class="fab fa-python text-blue-600 text-6xl"></i>
                    <p class="text-sm text-gray-600 mt-2">Python</p>
                </div>
                <div class="text-center">
                    <i class="fab fa-js-square text-yellow-500 text-6xl"></i>
                    <p class="text-sm text-gray-600 mt-2">JavaScript</p>
                </div>
                <div class="text-center">
                    <i class="fab fa-html5 text-orange-500 text-6xl"></i>
                    <p class="text-sm text-gray-600 mt-2">HTML5</p>
                </div>
                <div class="text-center">
                    <i class="fab fa-css3-alt text-blue-500 text-6xl"></i>
                    <p class="text-sm text-gray-600 mt-2">CSS3</p>
                </div>
                <div class="text-center">
                    <i class="fas fa-database text-gray-600 text-6xl"></i>
                    <p class="text-sm text-gray-600 mt-2">Database</p>
                </div>
                <div class="text-center">
                    <i class="fas fa-cloud text-blue-400 text-6xl"></i>
                    <p class="text-sm text-gray-600 mt-2">Cloud Infrastructure</p>
                </div>
            </div>
        </section>

        <!-- Attractive Charts Section: Uses Chart.js to render an illustrative bar chart -->
        <section class="mb-12">
            <h2 class="text-3xl font-bold text-gray-800 mb-6 section-header">
                Tool Usage Statistics (Illustrative)
            </h2>
            <p class="text-gray-700 mb-6">
                Below is an illustrative chart showcasing the hypothetical usage of our popular tools. Actual data may vary. This chart is generated dynamically using JavaScript.
            </p>
            <div class="bg-gray-50 p-6 rounded-lg shadow-inner">
                <canvas id="toolUsageChart" width="400" height="200"></canvas>
            </div>
        </section>

        <!-- Call to Action Section: Encourages users to visit the website -->
        <section class="text-center mb-12">
            <h2 class="text-3xl font-bold text-gray-800 mb-6 section-header inline-block">
                Ready to Simplify Your Excel Work?
            </h2>
            <p class="text-xl text-gray-700 mb-8">
                Visit XL-Factor today and experience the power of free, efficient, and user-friendly Excel tools.
            </p>
            <a href="https://www.xl-factor.com" target="_blank" class="inline-block btn-primary">
                Explore All Tools
            </a>
        </section>

        <!-- Footer: Copyright information and a friendly closing remark -->
        <footer class="text-center text-gray-500 text-sm mt-12 pt-8 border-t border-gray-200">
            <p>&copy; 2024 XL-Factor. All rights reserved.</p>
            <p>Made with <i class="fas fa-heart text-red-500 mx-1"></i> for data enthusiasts.</p>
        </footer>
    </div>

    <script>
        /*
         * JavaScript for generating the interactive chart using Chart.js.
         * This script runs once the DOM content is fully loaded.
         */
        document.addEventListener('DOMContentLoaded', function() {
            // Data for the bar chart, representing illustrative tool usage.
            const chartData = {
                labels: ['Excel Conversion', 'Merge Excel', 'Merge Sheet', 'Split Sheet', 'V Lookup', 'Image V Lookup'],
                datasets: [{
                    label: 'Monthly Usage (Illustrative)',
                    data: [1500, 900, 750, 600, 1100, 450], // Sample data points for each tool
                    backgroundColor: [
                        'rgba(75, 192, 192, 0.7)', // Greenish-blue for conversion
                        'rgba(153, 102, 255, 0.7)',// Purple for merge Excel
                        'rgba(255, 159, 64, 0.7)', // Orange for merge sheet
                        'rgba(255, 99, 132, 0.7)', // Red for split sheet
                        'rgba(54, 162, 235, 0.7)', // Blue for V Lookup
                        'rgba(201, 203, 207, 0.7)' // Gray for image V Lookup
                    ],
                    borderColor: [
                        'rgba(75, 192, 192, 1)',
                        'rgba(153, 102, 255, 1)',
                        'rgba(255, 159, 64, 1)',
                        'rgba(255, 99, 132, 1)',
                        'rgba(54, 162, 235, 1)',
                        'rgba(201, 203, 207, 1)'
                    ],
                    borderWidth: 1 // Border width for chart bars
                }]
            };

            // Options for the Chart.js configuration, controlling responsiveness, legends, and scales.
            const chartOptions = {
                responsive: true, // Chart will resize with its container
                maintainAspectRatio: false, // Allows height to be set independently of width
                plugins: {
                    legend: {
                        display: true, // Show the legend
                        position: 'top', // Position legend at the top
                        labels: {
                            color: '#333' // Color of legend labels
                        }
                    },
                    title: {
                        display: true, // Show the chart title
                        text: 'Popularity of XL-Factor Tools', // Chart title text
                        font: {
                            size: 18,
                            weight: 'bold'
                        },
                        color: '#333'
                    }
                },
                scales: {
                    y: {
                        beginAtZero: true, // Y-axis starts from zero
                        ticks: {
                            color: '#555' // Color of Y-axis ticks
                        },
                        grid: {
                            color: 'rgba(200, 200, 200, 0.2)' // Light grid lines on Y-axis
                        }
                    },
                    x: {
                        ticks: {
                            color: '#555' // Color of X-axis ticks
                        },
                        grid: {
                            color: 'rgba(200, 200, 200, 0.2)' // Light grid lines on X-axis
                        }
                    }
                }
            };

            // Get the canvas element where the chart will be drawn
            const ctx = document.getElementById('toolUsageChart');

            // Create the chart instance only if the canvas element is found
            if (ctx) {
                new Chart(ctx, {
                    type: 'bar', // Specifies a bar chart
                    data: chartData, // Assigns the data defined above
                    options: chartOptions // Assigns the options defined above
                });
            }
        });
    </script>
</body>
</html>
