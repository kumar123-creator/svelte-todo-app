<script>
	import Grid from "gridjs-svelte";
  
	const data = [
		['Mumbai Indians', 8, 6, 2, 0, 0, 12, 0.494],
    ['Chennai Super Kings', 7, 5, 2, 0, 0, 10, 1.263],
    ['Royal Challengers Bangalore', 7, 5, 2, 0, 0, 10, -0.171],
    ['Delhi Capitals', 8, 4, 4, 0, 0, 8, -0.055],
    ['Punjab Kings', 8, 4, 4, 0, 0, 8, -0.368],
    ['Kolkata Knight Riders', 7, 2, 5, 0, 0, 4, -0.494],
    ['Rajasthan Royals', 7, 2, 5, 0, 0, 4, -0.69],
    ['Sunrisers Hyderabad', 7, 1, 6, 0, 0, 2, -0.623],
  ];
  
	const columns = [];
  
  </script>
  
  <Grid data={data} 
  sort 
  search 
  pagination={{ enabled: true, limit: 3 }} columns={columns} />
 
  
  <style global>
	@import "https://cdn.jsdelivr.net/npm/gridjs/dist/theme/mermaid.min.css";
  </style>
