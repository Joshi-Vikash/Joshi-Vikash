- 👋 Hi, I’m @Joshi-Vikash
- 👀 I’m interested in technlogies around data and its insights 
- 🌱 I’m currently learning Spark and other Hadoop related technologies 
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
Joshi-Vikash/Joshi-Vikash is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
```
<div id="searchContainer" style="margin-bottom: 20px;">
  <input type="text" id="searchBox" placeholder="Search Title or Description" style="width: 300px; padding: 5px;" />
</div>
<script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
<script src="/sites/assets/customScript.js"></script>

```

```
<div id="searchContainer" style="margin-bottom: 20px;">
  <input type="text" id="searchBox" placeholder="Search Title or Description" style="width: 300px; padding: 5px;" />
</div>
<script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
<script>
  $(document).ready(function () {
    $("#searchBox").on("keyup", function () {
      const searchText = $(this).val().toLowerCase();
      $("tr.ms-itmhover").each(function () {
        const title = $(this).find("td:nth-child(2)").text().toLowerCase();
        const description = $(this).find("td:nth-child(3)").text().toLowerCase();
        if (title.includes(searchText) || description.includes(searchText)) {
          $(this).show();
        } else {
          $(this).hide();
        }
      });
    });
  });
</script>

```
