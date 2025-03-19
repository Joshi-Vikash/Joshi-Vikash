- 👋 Hi, I’m @Joshi-Vikash
- 👀 I’m interested in technlogies around data and its insights 
- 🌱 I’m currently learning Spark and other Hadoop related technologies 
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- $("div.ms-viewheadertr").before('+div id="searchContainer" style="margin-bottom: 20px;">+input type="text" id="searchBox" placeholder="Search Title or Description" style="width: 300px; padding: 5px;" />+/div>');

<!---
Joshi-Vikash/Joshi-Vikash is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->


<script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
<script>
  $(document).ready(function () {
    // Add a search box above the list
    $("#searchContainer").remove(); // Clear old search box if reloading script
   // $("div.ms-viewheadertr").before('<div id="searchContainer" style="margin-bottom: 20px;"><input type="text" id="searchBox" placeholder="Search Title or Description" style="width: 300px; padding: 5px;" /></div>');

    // Event listener for the search box
    $("#searchBox").on("keyup", function () {
      const searchText = $(this).val().toLowerCase();

      // Loop through each item in the list
      $("tr.ms-listviewtable").each(function () {
        const title = $(this).find("td:nth-child(2)").text().toLowerCase(); // Adjust column index for "Title"
        const description = $(this).find("td:nth-child(3)").text().toLowerCase(); // Adjust column index for "Description"

        // Show or hide rows based on the search query
        if (title.includes(searchText) || description.includes(searchText)) {
          $(this).show();
        } else {
          $(this).hide();
        }
      });
    });
  });
</script>

