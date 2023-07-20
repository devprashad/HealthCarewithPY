<!DOCTYPE html>
<html>
<body>
    <h1>Healthcare System with Merkle Tree and Bloom Filter</h1>
    <p>This is a simple healthcare system implementation in Python, using a Merkle Tree and Bloom Filter for secure and efficient data management. The system allows adding and searching medical records.</p>
    <h2>Prerequisites</h2>
    <ul>
        <li>Python 3.x</li>
        <li>tkinter library (usually included in Python standard library)</li>
    </ul>
    <h2>How it Works</h2>
    <h3>Merkle Tree</h3>
    <p>A Merkle Tree is a binary tree data structure used to efficiently verify the integrity of large datasets. In this system, we use a Merkle Tree to store and organize medical records in a tamper-evident manner. The tree is constructed by hashing individual medical records (leaves) and then hashing the resulting hashes until a single root hash is obtained. The root hash represents the entire dataset and serves as a unique identifier for it.</p>
    <h3>Bloom Filter</h3>
    <p>A Bloom Filter is a probabilistic data structure used for membership tests. It allows for quick and space-efficient checks to determine whether an element is likely to be present in a set. In this system, we use a Bloom Filter to check whether a medical record is present in the system before performing an expensive lookup in the Merkle Tree.</p>
    <h2>How to Use</h2>
    <ol>
        <li>Clone the repository or download the Python script.</li>
        <li>Ensure you have the required libraries installed (<code>hashlib</code> and <code>tkinter</code>).</li>
        <li>Run the script in your Python environment.</li>
        <li>The GUI will open, allowing you to interact with the healthcare system.</li>
    </ol>
    <h3>Adding Health Data</h3>
    <ul>
        <li>Enter the medical record information (Medical Record, Name, Age, Sugar Level, Blood Pressure) in the provided entry fields.</li>
        <li>Click on the "Add Health Data" button to add the record to the system.</li>
    </ul>
    <h3>Searching Health Data</h3>
    <ul>
        <li>Enter the medical record number in the "Search Medical Record" entry field.</li>
        <li>Click on the "Search" button to check if the medical record exists in the system.</li>
        <li>If the record is found, the details will be displayed in the text box below the search button.</li>
    </ul>
    <h3>Merkle Tree Visualization</h3>
    <p>The GUI will display the Merkle Tree structure after each addition of health data. The Merkle Tree is updated automatically with every new entry.</p> 
    <h2>Important Notes</h2>
    <ul>
        <li>The system uses SHA-256 hashing to secure the data and build the Merkle Tree.</li>
        <li>The Bloom Filter's false-positive rate is controlled by the 'error_rate' parameter. A smaller error rate means a larger bit array and more hash functions, which may increase memory usage.</li>
        <li>This implementation is meant for educational purposes and may not be suitable for production environments.</li>
    </ul>
</body>
</html>
