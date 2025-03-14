---
layout: default
title: "Data"
---

# Data Visualization

Here you will find interactive charts and graphs about European Parliament votes.

## Sample Chart
<canvas id="myChart"></canvas>

<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
<script>
    document.addEventListener("DOMContentLoaded", function () {
        const ctx = document.getElementById("myChart").getContext("2d");
        new Chart(ctx, {
            type: "bar",
            data: {
                labels: ["Party A", "Party B", "Party C"],
                datasets: [{
                    label: "Votes",
                    data: [12, 19, 7],
                    backgroundColor: "blue"
                }]
            }
        });
    });
</script>
