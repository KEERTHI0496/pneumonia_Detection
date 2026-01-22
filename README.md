<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Pneumonia Detection Using Deep Learning</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <style>
        body {
            font-family: Arial, Helvetica, sans-serif;
            line-height: 1.6;
            margin: 40px;
            background-color: #f9f9f9;
            color: #333;
        }

        h1, h2, h3 {
            color: #1a4d8f;
        }

        h1 {
            text-align: center;
            margin-bottom: 30px;
        }

        section {
            background: #ffffff;
            padding: 25px;
            margin-bottom: 20px;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0,0,0,0.08);
        }

        ul {
            margin-left: 20px;
        }

        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 15px;
        }

        table, th, td {
            border: 1px solid #ccc;
        }

        th, td {
            padding: 10px;
            text-align: center;
        }

        th {
            background-color: #1a4d8f;
            color: white;
        }

        img {
            max-width: 100%;
            height: auto;
            display: block;
            margin: 15px auto;
        }

        footer {
            text-align: center;
            margin-top: 40px;
            font-size: 14px;
            color: #666;
        }
    </style>
</head>

<body>

<h1>Pneumonia Detection Using Deep Learning</h1>

<section>
    <h2>Introduction</h2>
    <p>
        This project aims to study a public dataset on pneumonia detection based on a binary classification problem.
        Data visualization, deep learning models from scratch, transfer learning, and Grad-CAM visualization
        were implemented. A Docker-based web application was also developed.
    </p>
</section>

<section>
    <h2>Dataset</h2>
    <h3>Kaggle Dataset</h3>
    <p>
        Dataset source:
        <a href="https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia" target="_blank">
            Chest X-ray Pneumonia Dataset
        </a>
    </p>
    <p>
        The dataset contains 5,863 chest X-ray images divided into NORMAL and PNEUMONIA classes.
    </p>
</section>

<section>
    <h2>Methods</h2>

    <h3>Data Visualization</h3>
    <p>
        OpenCV, Matplotlib, and Seaborn were used for visualization.
        Canny edge detection was applied to enhance image edges.
    </p>

    <h3>Deep Learning Models</h3>
    <ul>
        <li>CNN Model built from scratch</li>
        <li>Transfer Learning using VGG-Face</li>
    </ul>
</section>

<section>
    <h2>Grad-CAM</h2>
    <p>
        Grad-CAM was used to visualize important lung regions contributing to pneumonia prediction.
        This improves model explainability.
    </p>
</section>

<section>
    <h2>Main Results</h2>

    <table>
        <tr>
            <th>Model</th>
            <th>Validation Accuracy</th>
        </tr>
        <tr>
            <td>Model from Scratch</td>
            <td>0.82</td>
        </tr>
        <tr>
            <td>Transfer Learning</td>
            <td>0.88</td>
        </tr>
    </table>
</section>

<section>
    <h2>Docker Application</h2>
    <p>
        A Docker-based Flask application allows users to upload X-ray images
        and receive predictions along with Grad-CAM heatmaps.
    </p>
</section>

<section>
    <h2>References</h2>
    <ol>
        <li>WHO – Pneumonia Statistics</li>
        <li>NHLBI – Pneumonia Diagnosis</li>
        <li>Parkhi et al., Deep Face Recognition</li>
        <li>DeepFace GitHub Repository</li>
    </ol>
</section>

<footer>
    <p>MCA Mini Project – Pneumonia Detection</p>
</footer>

</body>
</html>
