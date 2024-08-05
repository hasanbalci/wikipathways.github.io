---
title: Help Communities
redirect_from: /index.php/Help:WikiPathways_Portals
---
<h1>Community Page Overview</h1>
<p><a href="/browse/communities.html">Community pages</a> are defined by two separate files; a <b>Community page</b> describing the community, and a <b>Pathway list</b> defining the pathway list for the community. Creating a new community is as easy as creating these two files and adding them to the appropriate repositories, and making updates to an existing community similarly involves editing the two files for an existing community. The two files have specific requirements on format and content described below. Making edits requires:</p>
<ul>
    <li>A free <a href="https://www.github.com/" target="_blank">GitHub account</a>.</li>
    <li>If you have write access to to the relevant WikiPathways repos (<a href="https://github.com/wikipathways/wikipathways-database" target=_blank>wikipathways-database</a> and <a href="https://github.com/wikipathways/wikipathways.github.io" target=_blank>wikipathways.github.io</a>), you can simply commit your changes. If you <b>don't have write access</b>, you will need to clone the two repos locally:</li>
    <ol>
    <li>Clone <a href="https://github.com/wikipathways/wikipathways-database" target=_blank>wikipathways-database</a>.</li>
    <li>Clone <a href="https://github.com/wikipathways/wikipathways.github.io" target=_blank>wikipathways.github.io</a>.</li>
    <li>For wikipathways.github.io, refer to the <a href="https://github.com/wikipathways/wikipathways.github.io#readme">README</a> for instructions on how to build the site locally for testing purposes.</li>
    <li>You can edit the files (markdown and text) in any text editor, but a code editor is recommended, for example <a href="https://code.visualstudio.com/" target=_blank>Visual Studio Code</a>.</li>
    </ol>

</ul>
<hr>
<div id="create community">
<h2>Create or Edit a Community Page</h2>
<p>All Community pages are designed using the same template layout, and the content of each Community is defined in a markdown file in the <a href="https://github.com/wikipathways/wikipathways.github.io/tree/main/_communities" target=_blank>communities directory</a>. In order to be processed correctly by Jekyll, the markdown file must have a YAML <b>front matter</b> block at the beginning of the file, defining a set of custom variables. The front matter must be contained within a set of triple-dashed lines (---). After the front matter code, the file can contain additional html for custom content. The variables defined for WikiPathways Communities are:</p>
<ul>
<li>display-name: The name of the Community displayed on the <a href="https://wikipathways.org/browse/communities.html" target=_blank>Communities</a> page.</li>
<li><b>title</b>: The page title at the top of the page.</li>
<li><b>description</b>: Text describing the Community.</li>
<li><b>short-description</b>: One or two sentences describing the Community, displayed on the <a href="https://wikipathways.org/browse/communities.html" target=_blank>Communities</a> page.</li>
<li><b>logo</b>: a link to a png image (optional).</li>
<li><b>logo-link</b>: URL for an external resource (optional).</li>
<li><b>logo-height</b>: Override for the logo from the default height of 40px (optional).</li>
<li><b>support</b>: Text describing any funding support for the Community (optional).</li>
<li><b>contribute</b>: Text describing how to contribute to the community (optional).</li>
<li><b>community-tag</b>: The relevant community tag. This should match the filename of the text file with the list of Community pathways. The pathway display on the Community page is automatically generated based on this tag.</li>
<li><b>editors</b>: Community editors listed under <b>Contact</b>.</li>
<li><b>redirect_from</b>: Partial URL on the old WikiPathways site to redirect from.</li>
</ul>
<p>As an example, the below image shows the markdown for the <a href="https://wikipathways.org/communities/aop.html" target=_blank>Adverse Outcome Pathways</a> Community.<br /><br />
<img src="/assets/img/help/MarkdownExample.png" alt="Markdown Example" width="700">
</p>
<p>To create or edit a community page, make your changes on a local clone, or if you have write access you can use the GitHub web interface directly.</p>
<ol>
<li><b>Using a local clone of the wikipathways.github.io repo</b>: Create a new .md file for your community, or edit an existing file in the <b>communities</b> directory. See above for details on the format of the file. <b>Pro-tip: to create a .md new file, simply copy the contents of an existing file, paste into your new .md file, update the content to match your new community, and save as a new .md file</b>. Next, create a pull request for the main wikipathways.github.io repo.</li>
<li><b>Using GitHub web interface</b>: Access an existing Community profile from the WikiPathways website by clicking the <b>Edit community profile</b> button (pencil icon) next to the title of the Community at the top of the Community page (requires write access).</li>
</ol>
</div>
<hr>
<div id="update community">
<h2>Create or Edit the Community Pathway List</h2> 
<p>The pathway list defined for each Community is simply a flat file list of all WikiPathways Identifiers (WPIDs) relevant for that Community. The list of pathway IDs for each Community is stored in the wikipathways-database repository, in the <a href="https://github.com/wikipathways/wikipathways-database/tree/main/communities" target="_blank">communities directory</a>.</p>

<p>To create or edit the Community pathway list for a community, either make your changes on a local clone, or use the GitHub web interface directly (requires write access).</p>
<ol>
<li><b>Using a local clone of wikipathways-database repo</b>: In the <b>communities</b> directory, create a simple .txt file with the relevant WPIDs listed as <b>one column, no header</b>, or update an existing pathway list file.</li>
<li>Give the the .txt file a name that can also be used as the <b>community-tag</b>. <b>These two must be identical</b>. In the example above (AOP Community), the name of the pathway list file and the community-tag is "AOP".</li>
<li><b>Using GitHub web interface</b>: Access an existing Community pathway list from the WikiPathways website by clicking the <b>Edit community pathways</b> button (pencil icon) next to the Community Pathways section (requires write access).</li>
</ol>
</div>
