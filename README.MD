<h3>Simple steps, how to create the custom build / release task</h3>
<ol>

<li>Create a package 

    tfx extension create --manifest-globs vss-extension.json
</li>
<li>
Publish package to Marketplace using command line 

    tfx extension publish --manifest-globs your-manifest.json --share-with youraccount
    
 Or package can be publish using <a href="https://aka.ms/vsmarketplace-manage">Management Portal</a>
 Login if you already have account otherwise careate and and drag drop .vsix (package) file
 </li>
 <li>
    Once package file is uploaded share you extention to you account so that it become accesible click on three dot next to you extension 
    and click Share/Unshare.     
 </li>
  <li> 
    If you needed to create the new GUID to use it in the manifest file use powershell to generate one
    <code> [guid]::NewGuid() </code>this wil generate guid which can be used in the manifest file.
  </li>
</ol>
