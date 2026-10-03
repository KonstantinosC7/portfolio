---
layout: default
title: "Projects"
nav_active: projects
---

<link rel="stylesheet" href="{{ '/assets/css/style.css' | relative_url }}">

{% include topnav.html %}

<section class="section">
  <h1>Projects</h1>

  <div class="project-list">
<!-- TrainUp -->
    <article class="p-card">
      <img class="p-thumb" src="{{ '/assets/img/TrainUp/TrainUp.jpg' | relative_url }}" alt="TrainUp">
      <div class="p-body">
        <h3>TrainUp — Traineeship Matching</h3>
      The aim of this project is to create an application that will help the University's Internship Committee monitor and manage both available and already assigned internship positions.   The application will mainly involve students, companies advertising positions, professors acting as supervisors, and the Committee overseeing the entire process.
        <ul class="p-bullets">
          <li>Committee workflow: roles, matching flow, notifications.</li>
          <li>Track available & assigned internship positions.</li>
        </ul>
        <p class="p-tech">Spring Boot, Thymeleaf, MySQL, HTML/CSS/Bootstrap</p>
        <div class="p-actions">
          <a class="btn small" href="https://github.com/KonstantinosC7/TrainUp" target="_blank">Repo</a>
          <a class="btn small ghost" href="https://github.com/KonstantinosC7/TrainUp/blob/main/reports/Project-description-v1.0.pdf" target="_blank">Report (PDF)</a>
        </div>
      </div>
    </article>

<!-- Diploma Projects Management App (Spring Boot) -->
<article class="p-card">
  <img class="p-thumb" src="{{ '/assets/img/ThesisLink/ThesisLink.png' | relative_url }}" alt="Diploma Projects Management App">
  <div class="p-body">
    <h3>Diploma Projects Management</h3>
    The goal of this project is to develop a web application that allows students to browse available thesis topics from various professors and apply for the thesis topics that interest them. The application also allows professors to assign thesis topics to students, supervise the thesis work assigned to them, and evaluate the results.
    <ul class="p-bullets">
      <li>Auth (login/register) with role-based views. </li> 
      <li>CRUD for profiles, subjects, applications, theses. </li>
      <li>UML-driven layered design (DAO/Service/Controller). </li>
    </ul>
    <p class="p-tech">Spring Boot (MVC + Security), Thymeleaf, MySQL, JPA, UML, Maven</p>
    <div class="p-actions">
      <a class="btn small" href="https://github.com/KonstantinosC7/Thesis-Link" target="_blank">Repo</a>
      <a class="btn small ghost" href="{{ '/assets/reports/SprintReport_v1.pdf' | relative_url }}" target="_blank">Sprint Report (PDF)</a>
    </div>
  </div>
</article>

<!-- SpecFlow (Spring Boot) -->
<article class="p-card">
  <img class="p-thumb" src="{{ '/assets/img/SpecFlow/logo.png' | relative_url }}" alt="SpecFlow">
  <div class="p-body">
    <h3>SpecFlow - Requirements Specification & Analysis Application</h3>
    This project develops a web-based Requirements Specification and Analysis application that supports collaborative software requirements definition and object-oriented analysis. Users can create structured Use Cases, generate CRC cards, link requirements to system components, and automatically export diagram scripts for tools such as PlantUML and Nomnoml. The platform bridges requirements gathering and software design in a secure and user-friendly environment. 
    <ul class="p-bullets">
      <li>Auth (login/register) with role-based views.</li>  
      <li>CRUD for profiles, Projects, Use Cases, CRC Cards.</li> <li>UML-driven layered design (DAO/Service/Controller)</li> 
      <li>Script for generating Diagrams.</li>
    </ul>
    <p class="p-tech">Spring Boot (MVC + Security), Thymeleaf, MySQL, JPA, UML, Maven</p>
    <div class="p-actions">
      <a class="btn small" href="https://github.com/KonstantinosC7/SpecFlow" target="_blank">Repo</a>
      <a class="btn small ghost" href="{{ '/assets/reports/SprintReport_v1_SpecFlow.pdf' | relative_url }}" target="_blank">Sprint Report (PDF)</a>
    </div>
  </div>
</article>
    
<!-- Information Retrieval (Songs Search) -->
  <article class="p-card">
    <img class="p-thumb" src="{{ '/assets/img/Informationretrieval/Information-Retrieval.jpg' | relative_url }}" alt="Information Retrieval UI (songs search)">
    <div class="p-body">
      <h3>Information Retrieval — Songs Search Engine</h3>
      <ul class="p-bullets">
        <li>Indexes song data from CSV with <strong>Apache Lucene</strong>; fast keyword search.</li>
        <li>Filters by <em>Artist</em>, <em>Song</em>, or <em>Lyrics</em> with optional <em>Alphabetical Grouping</em>.</li>
        <li>Web view with query history, ranked results, and full-lyrics page (next/prev).</li>
      </ul>
      <p class="p-tech">Java, Apache Lucene, CSV parsing, Web UI</p>
      <div class="p-actions">
        <a class="btn small" href="https://github.com/KonstantinosC7/InformationRetrieval" target="_blank">Repo</a>
        <!-- Option A: link to the PDF in GitHub -->
        <a class="btn small ghost" href="https://github.com/KonstantinosC7/InformationRetrieval/blob/main/Report_Information_Retrieval.pdf" target="_blank">Report (PDF)</a>
    </div>
  </div>
</article>

<!-- MLP Classifier (Java) -->
<article class="p-card">
  <img class="p-thumb" src="{{ '/assets/img/MLP/MLP_Screenshot.png' | relative_url }}" alt="MLP Classifier — test set classification">
  <div class="p-body">
    <h3>MLP Classifier — Neural Network from Scratch</h3>
    A Multi-Layer Perceptron with three hidden layers, implemented from scratch in Java (no ML libraries) to classify points in a 2D plane into three categories with non-linear decision boundaries. The network is trained with mini-batch gradient descent and backpropagation, and its generalization is studied across hidden-layer sizes, activation functions and batch sizes.
    <ul class="p-bullets">
      <li>Configurable architecture (H1/H2/H3), activations (logistic, tanh, ReLU) and batch size.</li>
      <li>Softmax output layer with one-hot targets; stopping rule on error change after at least 700 epochs.</li>
      <li>Best result: <strong>92.4% test accuracy</strong> (28-28-30 neurons, tanh, B=40).</li>
    </ul>
    <p class="p-tech">Java, Backpropagation, Gradient Descent, Softmax, Python (matplotlib)</p>
    <div class="p-actions">
      <a class="btn small" href="https://github.com/KonstantinosC7/mlp-classifier-java" target="_blank">Repo</a>
      <a class="btn small ghost" href="https://github.com/KonstantinosC7/mlp-classifier-java/blob/main/docs/MLP_report.pdf" target="_blank">Report (PDF)</a>
    </div>
  </div>
</article>

<!-- Monster Type Recognition (Classifier Comparison) -->
<article class="p-card">
  <img class="p-thumb" src="{{ '/assets/img/MonsterClassification/kaggle_accuracy.png' | relative_url }}" alt="Monster Type Recognition — Kaggle accuracy by classifier">
  <div class="p-body">
    <h3>Monster Type Recognition — Classifier Comparison</h3>
    A comparative study of four classic machine-learning classifiers on the Kaggle dataset "Ghouls, Goblins, and Ghosts... Boo!", where the goal is to recognise a monster's type (Ghoul, Goblin or Ghost) from five features. Every model is evaluated with accuracy, F1, precision and recall, and its predictions are scored on Kaggle.
    <ul class="p-bullets">
      <li>k-NN (k = 1, 3, 5, 10), neural networks (1–2 sigmoid hidden layers, softmax output, SGD) and linear/RBF SVMs with one-versus-rest.</li>
      <li>Naive Bayes written from scratch: normal distribution for the continuous features, multinomial for the color.</li>
      <li>Best result: <strong>0.73156 Kaggle accuracy</strong> (linear SVM, C=10).</li>
    </ul>
    <p class="p-tech">Python, scikit-learn, TensorFlow/Keras, pandas, NumPy</p>
    <div class="p-actions">
      <a class="btn small" href="https://github.com/KonstantinosC7/Monster-Classifiers" target="_blank">Repo</a>
      <a class="btn small ghost" href="https://github.com/KonstantinosC7/Monster-Classifiers/blob/main/docs/report.pdf" target="_blank">Report (PDF)</a>
    </div>
  </div>
</article>

<!-- Finding Similar Documents with MinHash and LSH -->
<article class="p-card">
  <img class="p-thumb" src="{{ '/assets/img/MinHashLSH/MinHashLSH.png' | relative_url }}" alt="MinHash and LSH">
  <div class="p-body">
    <h3>MinHash & LSH — Similar Document Search</h3>
    A Big Data project that implements and compares different approaches for finding the most similar documents in large collections. Documents are represented as sets of words, with Jaccard similarity used as the ground truth and MinHash signatures used to efficiently estimate similarity. Locality Sensitive Hashing (LSH) is then used to reduce the number of document comparisons and improve search efficiency.
    <ul class="p-bullets">
      <li>Implemented brute-force Jaccard and MinHash similarity for nearest-neighbor search.</li>
      <li>Built MinHash signature matrices using randomized hash functions and an inverted index.</li>
      <li>Implemented LSH banding to generate candidate document pairs and reduce comparisons.</li>
      <li>Compared methods using execution time and average similarity on Enron emails and NIPS papers.</li>
    </ul>
    <p class="p-tech">Python, MinHash, Locality Sensitive Hashing (LSH), Jaccard Similarity, Big Data Algorithms</p>
    <div class="p-actions">
      <a class="btn small" href="https://github.com/KonstantinosC7/Algorithms_for_Large-Scale_Data" target="_blank">Repo</a>
    </div>
  </div>
</article>


<footer class="footer">
  <span>© {{ site.time | date: '%Y' }} Konstantinos Christopoulos</span>
</footer>
