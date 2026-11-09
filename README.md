<h1>Setting Up Your Workflow</h1>

<p>EthPillar guides are created using <a href="https://docusaurus.io/" target="_blank">Docusaurus</a>, a project by <a href="https://opensource.fb.com/projects/docusaurus/" target="_blank">Meta Open Source</a> designed for building optimized Web sites quickly. Built using <a href="https://nodejs.org/en" target="_blank">Node.js<sup>®</sup></a> and <a href="https://react.dev/" target="_blank">React</a>, Docusaurus is platform agnostic.</p>

<p>To edit the guides, <a href="https://CoinCashew.io" target="_blank">CoinCashew.io</a> recommends using the <a href="https://code.visualstudio.com/" target="_blank">Visual Studio Code</a> source code editor.</p>

<p>To set up a workflow for revising the EthPillar guides, you need to:</p>

<ul>
  <li>Install Node.js and Docusaurus</li>
  <li>Download the GitHub repository for the EthPillar guides</li>
  <li>Install and configure the Visual Studio Code editor</li>
</ul>

<h2>Installing Node.js</h2>

<p>Node.js is an open-source, cross-platform JavaScript runtime environment that executes JavaScript code outside of a Web browser.</p>

<p><strong>To install Node.js:</strong></p>

<ul>
  <li>Using a Web browser, visit the <a href="https://nodejs.org/en/download/" target="_blank">Download Node.js</a> page. In the dropdown fields, select a Node.js Long-Term Support (LTS) version 18.0 or above for your operating system using <b>nvm</b> with <b>npm</b>, and then follow the instructions that the Download page displays.<br />
    <div align="center"><strong>OR</strong></div>
    Download a prebuilt Node.js installer for your operating system, then run then installer, and then follow the instructions on screen to complete the installation.</li>
</ul>

<h2>Installing and Starting Docusaurus</h2>

<p>The simplest method of installing Docusaurus involves creating a new project Web site using a default template.</p>

<p><strong>To install Docusaurus:</strong></p>

<ol>
  <li>Using a terminal window, navigate to the folder where you want to store Docusaurus project Web sites, such as the EthPillar guides.</li>
  <li>To create a new Docusaurus project Web site, type the following command where <code>&lt;WebsiteName&gt;</code> is the name of the new project:<br />
    <code>npx create-docusaurus@latest &lt;WebsiteName&gt; classic</code></li>
  <li>When prompted to install the <code>create-docusaurus</code> package, type <code>y</code> and then press <code>ENTER</code>to proceed.</li>
  <li>When prompted to select a language, select <code>JavaScript</code> and then press <code>ENTER</code></li>
  <li>When the installation completes, to start the development server for the new project Web site, type:<br />
    <code>cd ./&lt;WebsiteName&gt;
npx docusaurus start</code></li>
</ol>

<p>The development server starts, and then compiles the Web site. The development server serves your Web site, allowing you to preview changes as you edit the files. When compiled successfully, your default Web browser opens displaying the Web site at <code>http://localhost:3000</code></p>
        
<p>For details on the folders and files comprising a Docusaurus Web site, refer to the <a href="https://docusaurus.io/docs/installation#project-structure" target="_blank">Project Structure</a>.</p>

<p>Use the project that you create as a playground to learn how to use Docusaurus.</p>

> [!NOTE]
> For more details on using Docusaurus, see the [documentation](https://docusaurus.io/docs).

<p><strong>To stop the development server:</strong></p>

<ol>
  <li>When you are finished your session editing the Web site, navigate to the terminal window running the development server, and then press <code>CTRL+C</code></li>
  <li>If prompted, confirm that you want to stop the development server.</li>
</ol>

<h2>Downloading and Compiling EthPillar Guides</h2>

<p>The <a href="https://github.com/CoinCashewIO/EthPillarGuides" target="_blank">EthPillarGuides</a> GitHub repository stores the source files for EthPillar guides—a fully open-source project fully powered by Ehtereum node operators like you.</p>

<p><strong>To download and compile the EthPillar guides:</strong></p>

<ol>
  <li>To install Git, if you are using Linux then type the following commands using a terminal window:<br />
    <code>sudo apt-get update
sudo apt-get install git</code><br />
    <div align="center"><strong>OR</strong></div>
    If you are using Windows, <a href="https://git-scm.com/downloads" target="_blank">download</a> a Standalone Installer, then run the EXE file that you downloaded, and then follow the instructions on screen to complete the installation.</li>
  <li>To configure Git, using a terminal window type the following commands where <code>&lt;UserName&gt;</code> is your Git user name, and <code>&lt;EmailAddress&gt;</code> is your e-mail address:<br />
    <code>git config --global user.name "<UserName>"
git config --global user.email "<EmailAddress>"</code> </li>

> [!NOTE]
> To display the current user name or e-mail address, type <code>git config --global user.name</code> or <code>git config --global user.email</code> respectively.








  
        <li>Using a Web browser, log in to your <a href="https://github.com/" target="_blank">GitHub</a> account.</li>
        <li>Navigate to the <a href="https://github.com/CoinCashewIO/CardanoSPOGuide" target="_blank">CardanoSPOGuide</a> repository, then click the <b>Fork</b> button, and then scroll down to click the green <b>Create Fork</b> button.</li>

        <li>Using a terminal window, navigate to the folder on your computer where you store Docusaurus project Web sites, and then type the following commands where <code>&lt;ForkedRepository&gt;</code> is the URL to the fork of the CardanoSPOGuide repository that you created in step 4:
          <CodeBlock language="bash">
            {`git clone <ForkedRepository>
cd ./CardanoSPOGuide
npm install
npm update
npm audit fix
`}
          </CodeBlock>
        </li>
        <li>To start the development server for the Guide, type <code>npx docusaurus start</code></li>
        <li>When you are ready to stop the development server, navigate to the terminal window running the development server, and then press <code>CTRL+C</code></li>
      </ol>

      <p>When revising the <i>How to Set Up a Cardano Stake Pool</i> guide, you need to know about the following folders and files in the Docusaurus project, relative to the root <code>CardanoSPOGuide</code> folder:</p>

      <ul>
        <li><code>/assets/</code>—Contains source files for images; scripts; and, snippets that you may use when revising the Guide</li>
        <li><code>/docs/</code>—Contains the content files for the Guide</li>
        <li><code>/src/css/custom.css</code>—Defines the Cascading Style Sheets (CSS) describing presentation and styling of the Guide</li>
        <li><code>/static/img/</code>—Contains image files that the Guide uses</li>
      </ul>

      <table class="box">
        <tbody>
          <tr>
            <td class="boxLabel"><p class="boxLabel">Note<br /><img src={useBaseUrl('img/BoxNote.png')} alt="Note" /></p></td>
            <td class="boxText"><p class="boxText">Specifying file paths relative to the root folder of the project is standard for Web sites created using Docusaurus.</p></td>
          </tr>
        </tbody>
      </table>

      <p>For details on creating a pull request to submit content that you create to CoinCashew for publication in the Guide, see the topic <a href="https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork" target="_blank">Creating a Pull Request from a Fork</a>.</p>

      <h2>Installing and Configuring Visual Studio Code</h2>

      <p>Visual Studio Code (VS Code) is a free, lightweight and powerful source code editor developed by Microsoft for Windows, macOS and Linux. VS Code is highly customizable and user friendly, offering features such as syntax highlighting, intelligent code completion and Git integration.</p>

      <p class="pi">To install and configure VS Code:</p>

      <ol>
        <li>Visit <a href="https://code.visualstudio.com/docs/setup/setup-overview" target="_blank">Setting Up Visual Studio Code</a>, and then follow the instructions for your platform.</li>
        <li>After finishing the installation, open VS Code</li>
        <li>In VS Code, click the <b>File</b> menu, then click <b>Open Folder</b>, then navigate to the <b>CardanoSPOGuide</b> folder, and then click <b>Open</b></li>
        <li>To install HTML code snippets for the Guide:
          <ol>
            <li>In the <b>Explorer</b> left pane, click to expand the <b>assets/text</b> subfolder, and then click to open the file <b>html-snippets.json</b></li>
            <li>Position the cursor in the <b>html-snippets.json</b> file, then press <b>CTRL+A</b>, and then press <b>CTRL+C</b> to copy the contents of the file.</li>
            <li>Click the <b>File</b> menu, then click <b>Preferences</b>, and then click <b>Configure Snippets</b></li>
            <li>In the <b>Select Snippets File</b> field, type <b>HTML</b>, and then press <b>ENTER</b></li>
            <li>In the <b>html.json</b> file that opens, position the cursor where you want to paste snippet definitions, then press <b>CTRL+V</b>, then edit the file as needed, and then press <b>CTRL+S</b> to save the html.json file.</li>
          </ol>
        </li>
        <li>To set the default Language Mode for files having the MDX file name extension to HTML:
          <ol>
            <li>Click the <b>File</b> menu, then click <b>Preferences</b>, and then click <b>Settings</b></li>
            <li>In the <b>Search Settings</b> field, type <b>files.associations</b></li>
            <li>In the <b>Files: Associations</b> setting, click the <b>Add Item</b> button. In the <b>Item</b> field type <b>*.mdx</b>, then in the <b>Value</b> field type <b>html</b>, and then click <b>OK</b></li>
          </ol>
        </li>
      </ol>

      <p>For details on using VS Code to submit content that you create to your fork of the CardanoSPOGuide repository, see the section <a href="https://code.visualstudio.com/docs/sourcecontrol/intro-to-git#_staging-and-committing-code-changes" target="_blank">Staging and Committing Code Changes</a>.</p>
