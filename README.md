<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cultural Heritage Data System</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
            background-color: #f8f9fa;
        }

        h1, h2, h3 {
            color: #2c3e50;
            border-bottom: 2px solid #3498db;
            padding-bottom: 5px;
        }

        code {
            background-color: #e9ecef;
            padding: 2px 5px;
            border-radius: 3px;
        }

        pre {
            background-color: #e9ecef;
            padding: 15px;
            border-radius: 5px;
            overflow-x: auto;
        }

        table {
            width: 100%;
            border-collapse: collapse;
            margin: 20px 0;
        }

        th, td {
            border: 1px solid #dee2e6;
            padding: 8px;
            text-align: left;
        }

        th {
            background-color: #3498db;
            color: white;
        }

        tr:nth-child(even) {
            background-color: #f8f9fa;
        }

        .license {
            background-color: #fff3cd;
            padding: 15px;
            border-radius: 5px;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <h1>Cultural Heritage Data Management System 🏛️</h1>

    <h2 id="requirements">📋 Requirements</h2>
    <ul>
        <li>Java 17+</li>
        <li>Maven 3.6+</li>
        <li>Data file <code>Archeologia---Storia-e-Tradizioni---Regione-Marche.csv</code></li>
        <li>UTF-8 encoding for all text files</li>
    </ul>

    <h2 id="installation">🚀 Installation</h2>
    <pre><code># Clone repository
git clone https://github.com/yourusername/cultural-heritage-system.git
cd cultural-heritage-system

# Build project
mvn clean package</code></pre>

    <h2 id="usage">🖥️ Usage</h2>
    <h3>Start Server</h3>
    <pre><code>java -jar target/heritage-server.jar</code></pre>

    <h3>Start Client</h3>
    <pre><code>java -jar target/heritage-client.jar</code></pre>

    <h3>Connection Defaults</h3>
    <table>
        <tr><th>Parameter</th><th>Value</th></tr>
        <tr><td>Server Address</td><td><code>localhost</code></td></tr>
        <tr><td>Port</td><td><code>12345</code></td></tr>
    </table>

    <h2 id="command-reference">⌨️ Command Reference</h2>
    <h3>Basic Commands</h3>
    <table>
        <tr><th>Command</th><th>Description</th></tr>
        <tr><td><code>HELP</code></td><td>Show command reference</td></tr>
        <tr><td><code>END</code></td><td>Disconnect from server</td></tr>
    </table>

    <h3>Search Operations</h3>
    <pre><code>SEARCH [OPTION] "QUERY"</code></pre>
    <table>
        <tr><th>Option</th><th>Search Type</th><th>Example</th></tr>
        <tr><td><code>-n</code></td><td>Exact name</td><td><code>SEARCH -n "Castelldimezzo"</code></td></tr>
        <tr><td><code>-c</code></td><td>Exact city</td><td><code>SEARCH -c Ancona</code></td></tr>
        <tr><td><code>-t</code></td><td>Exact type</td><td><code>SEARCH -t Archeologia</code></td></tr>
        <tr><td><code>-a</code></td><td>Exact address</td><td><code>SEARCH -a "Via Ferretti"</code></td></tr>
        <tr><td><code>--n</code></td><td>Partial name</td><td><code>SEARCH --n castle</code></td></tr>
        <tr><td><code>--c</code></td><td>Partial city</td><td><code>SEARCH --c piceno</code></td></tr>
        <tr><td><code>--t</code></td><td>Partial type</td><td><code>SEARCH --t paesaggio</code></td></tr>
        <tr><td><code>--a</code></td><td>Partial address</td><td><code>SEARCH --a piazza</code></td></tr>
        <tr><td><code>-o</code></td><td>Opening days</td><td><code>SEARCH -o lunedì</code></td></tr>
    </table>

    <h2 id="data-format">📊 Data Format</h2>
    <pre>ImageURL;Caption;Type;Name;City;Address;Number;Phone;Email;Website;Latitude;Longitude;OpeningHours</pre>

    <h2 id="troubleshooting">🛠️ Troubleshooting</h2>
    <h3>Common Issues</h3>
    <table>
        <tr><th>Error</th><th>Solution</th></tr>
        <tr><td>Connection failed</td><td>Verify server is running</td></tr>
        <tr><td>Invalid command format</td><td>Check command syntax</td></tr>
        <tr><td>Index out of bounds</td><td>Use valid index (0 ≤ index < dataset size)</td></tr>
    </table>

    <h2 id="license">📄 License</h2>
    <div class="license">
        This project is licensed under the MIT License - see the 
        <a href="LICENSE">LICENSE</a> file for details.<br><br>
        <em>Academic Project - Not for Commercial Use</em>
    </div>
</body>
</html>
