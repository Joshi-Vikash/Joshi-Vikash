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

```

```
<script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
<script>
  $(document).ready(function () {
    // Add search box above the list
    $("#searchContainer").remove(); // Ensure no duplicate search containers
    $("div.ms-viewheadertr").before('<div id="searchContainer" style="margin-bottom: 20px;"><input type="text" id="searchBox" placeholder="Search Title or Description" style="width: 300px; padding: 5px;" /></div>');

    // Search functionality
    $("#searchBox").on("keyup", function () {
      const searchText = $(this).val().toLowerCase();

      // Loop through each group header and its child rows
      $(".ms-gb").each(function () {
        const groupHeader = $(this); // The category row
        let hasMatch = false; // Track if a match is found within the group

        // Check all rows in the group
        const groupItems = groupHeader.nextUntil(".ms-gb"); // Select rows until the next group header
        groupItems.each(function () {
          const title = $(this).find("td:nth-child(2)").text().toLowerCase(); // Adjust column index for Title
          const description = $(this).find("td:nth-child(3)").text().toLowerCase(); // Adjust column index for Description

          if (title.includes(searchText) || description.includes(searchText)) {
            $(this).show(); // Show matching row
            hasMatch = true; // Mark that there's a match in this group
          } else {
            $(this).hide(); // Hide non-matching row
          }
        });

        // Show or hide the group header based on whether there's a match
        if (hasMatch) {
          groupHeader.show();
        } else {
          groupHeader.hide();
        }
      });
    });
  });
</script>

```
