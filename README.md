
<h2>Social Media -- FakeBook</h2>

<li>Introduction - the aim of the webpage</li>
<li>Technologies</li>
<li>Key Code</li>
<li>Launch</li>
<li>Reference</li>

<h3>Introduction - the project's aim</h3>
<p>
    This page is used to imitate the post page of Facebook, the header and the post operation, users could choose file and upload the images and post it on the timeline. Clicking the avatar on the top right, you will get the basic information of this user, including user's ID, name, username and email, click for the second time, the information will disappear.
</p>


<h3>Technologies</h3>
<li>HTML5</li>
<li>CSS3</li>
<li>Git</li>

<h3>key Code</h3>

```
    let postBtn = document.querySelector('.postbtn');
    let postInputContent = document.querySelector('.post-input-content')
    postBtn.addEventListener('click', function() {
        let photo = file.files;
        let div = document.createElement('div');
        let item = document.querySelector('.post-content');
        let reader = new FileReader();
        item.insertBefore(div, item.children[0]);
        reader.readAsDataURL(photo[0]);
        reader.onload = function () {
        let image = document.createElement('img');
        image.width = '450';
        image.src = reader.result; 
        let items = document.querySelector('.post-content div');
        items.append(image);
    }
```

<h3>Launch</h3>
<p>This webpage is prepared to launch, users can click the link to preview it.</p>
<a href="https://bricklai.github.io/social-media/index.html">Click here</a> to view the webpage

