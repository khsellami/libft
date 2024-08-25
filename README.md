<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>C Library Project - README</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            color: #333;
            background-color: #f4f4f4;
            margin: 0;
            padding: 0;
        }
        .container {
            width: 80%;
            margin: auto;
            overflow: hidden;
        }
        header {
            background: #333;
            color: #fff;
            padding-top: 10px;
            min-height: 50px;
            border-bottom: #fff 3px solid;
            margin-bottom: 20px;
        }
        header h1 {
            text-align: center;
            margin: 0;
        }
        h2 {
            color: #333;
        }
        code {
            background: #e2e2e2;
            padding: 2px 4px;
            border-radius: 4px;
        }
        pre {
            background: #e2e2e2;
            padding: 10px;
            border-radius: 4px;
            overflow-x: auto;
        }
        ul {
            list-style: none;
            padding: 0;
        }
        li {
            margin: 10px 0;
        }
        .section {
            background: #fff;
            padding: 20px;
            border-radius: 4px;
            margin-bottom: 20px;
        }
        footer {
            background: #333;
            color: #fff;
            padding: 10px;
            text-align: center;
            border-top: #fff 3px solid;
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <h1>C Library Project - README</h1>
        </div>
    </header>

    <div class="container">
        <div class="section">
            <h2>Project Overview</h2>
            <p>This project involves creating a C library that contains a collection of general-purpose functions to be used by your programs. The library should be written in C and adhere strictly to the provided guidelines and norms. It will be evaluated on several criteria, including code quality, adherence to standards, and functionality.</p>
        </div>

        <div class="section">
            <h2>Project Requirements</h2>
            <ul>
                <li><strong>Code Quality and Norm Compliance</strong> - All code must comply with the Norm (a set of coding standards). Any bonus files/functions are included in the norm check, and norm errors will result in a score of 0.</li>
                <li><strong>Error Handling</strong> - Functions must not crash unexpectedly (e.g., segmentation faults, bus errors, double frees). Proper error handling should be implemented, and undefined behaviors must be managed appropriately.</li>
                <li><strong>Memory Management</strong> - All heap-allocated memory must be properly freed to avoid memory leaks. Memory management issues will result in a non-functional project and a score of 0.</li>
                <li><strong>Makefile Requirements</strong> - Submit a <code>Makefile</code> with rules for <code>$(NAME)</code>, <code>all</code>, <code>clean</code>, <code>fclean</code>, and <code>re</code>. Ensure the <code>Makefile</code> compiles the source files with the flags <code>-Wall</code>, <code>-Wextra</code>, and <code>-Werror</code>, and uses <code>cc</code>. The <code>Makefile</code> should not relink files unnecessarily.</li>
                <li><strong>Bonus Features</strong> - If applicable, include a <code>bonus</code> rule in your <code>Makefile</code> to handle bonus features. Bonus files should be in a separate <code>_bonus.{c/h}</code> file. Mandatory and bonus parts are evaluated separately.</li>
                <li><strong>Libft Integration</strong> - If the project allows the use of <code>libft</code>, copy its sources and <code>Makefile</code> into a <code>libft</code> folder. Your <code>Makefile</code> should compile <code>libft</code> using its own <code>Makefile</code>, then compile the project.</li>
                <li><strong>Testing</strong> - Although testing programs are not submitted, they are highly recommended to ensure the correctness of your library. Create tests for each function in your library to validate their behavior and edge cases.</li>
                <li><strong>Submission</strong> - Submit your work to the assigned git repository. Only the work in the git repository will be graded. If Deepthought is used for grading, any errors will halt the evaluation process.</li>
            </ul>
        </div>

        <div class="section">
            <h2>Directory Structure</h2>
            <pre>
/project-root
|-- src/            # Source files for your library
|-- include/        # Header files for your library
|-- libft/          # Directory for libft, if applicable
|   |-- src/        # Source files for libft
|   |-- include/    # Header files for libft
|   |-- Makefile    # Makefile for libft
|-- tests/          # Test programs (not submitted)
|-- Makefile        # Main Makefile for the project
|-- README.md       # This README file
            </pre>
        </div>

        <div class="section">
            <h2>Makefile Rules</h2>
            <ul>
                <li><code>$(NAME)</code> - Compiles the library and produces the final output.</li>
                <li><code>all</code> - Builds the project and all its dependencies.</li>
                <li><code>clean</code> - Removes object files and other temporary files.</li>
                <li><code>fclean</code> - Removes all files created by the <code>all</code> and <code>clean</code> rules, including the final output.</li>
                <li><code>re</code> - Rebuilds the project from scratch.</li>
                <li><code>bonus</code> - Includes rules for compiling bonus features, if applicable.</li>
            </ul>
        </div>

        <div class="section">
            <h2>Usage</h2>
            <p>To build your project, run:</p>
            <pre><code>make</code></pre>
            <p>To clean up temporary files, run:</p>
            <pre><code>make clean</code></pre>
            <p>To remove all built files and start from scratch, run:</p>
            <pre><code>make fclean</code></pre>
            <p>To rebuild the project, run:</p>
            <pre><code>make re</code></pre>
            <p>If you have bonus features, compile them with:</p>
            <pre><code>make bonus</code></pre>
        </div>

        <div class="section">
            <h2>Contact</h2>
            <p>For any questions or clarifications, please refer to the project's documentation or contact your project supervisor.</p>
        </div>
    </div>

    <footer>
        <p>&copy; 2024 C Library Project. All rights reserved.</p>
    </footer>
</body>
</html>
