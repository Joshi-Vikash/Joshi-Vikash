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
// Ensure the script runs after the DOM has fully loaded
$(document).ready(function () {
  // Attach a keyup event to the search box
  $("#searchBox").on("keyup", function () {
    // Get the search query
    const searchText = $(this).val().toLowerCase();

    // Loop through each row in the SharePoint list
    $("tr.ms-itmhover").each(function () {
      // Find the Title and Description columns (adjust column indexes if needed)
      const title = $(this).find("td:nth-child(2)").text().toLowerCase(); // Title column
      const description = $(this).find("td:nth-child(3)").text().toLowerCase(); // Description column

      // Show or hide rows based on the search query
      if (title.includes(searchText) || description.includes(searchText)) {
        $(this).show(); // Show row if it matches
      } else {
        $(this).hide(); // Hide row if it doesn't match
      }
    });
  });
});
```
