---
showonlyimage: true
title: "Dates"
subtitle: "Workshop paper submission and notification"
excerpt: "Dates"
description: "The call for papers is out"
date: 2024-06-16
author: "Gianluca Aguzzi, Sara Montagna, Mauro Dragoni"
URL: "/dates"
---

<style>
.past-date {
    color: gray;
    text-decoration: line-through;
}

.approaching-deadline {
    color: orange;
    font-weight: bold;
}
</style>

<script>
document.addEventListener('DOMContentLoaded', function() {
    const deadlines = document.querySelectorAll('.deadline');

    deadlines.forEach(deadline => {
        const dateStr = deadline.dataset.date;
        const deadlineDate = new Date(dateStr);
        const now = new Date();
        const timeDiff = deadlineDate.getTime() - now.getTime();
        const daysRemaining = Math.ceil(timeDiff / (1000 * 3600 * 24));

        if (daysRemaining < 0) {
            deadline.classList.add('past-date');
        } else if (daysRemaining <= 7) {
            deadline.classList.add('approaching-deadline');
        }
    });
});
</script>

# Dates
* **Paper submission deadline**: <span class="deadline yellow" data-date="2025-04-19">April 24th, 2025</span>

* **Paper notification**: <span class="deadline yellow" data-date="2025-05-15">May 15th, 2025</span>

* **Camera ready deadline**: <span class="deadline yellow" data-date="2025-06-06">June 6th, 2025</span>

* **Workshop**: <span class="deadline yellow" data-date="2025-06-20">June 26th, 2025</span>

<!--
# Dates
* Paper submission deadline: 
~~November 17th, 2024~~ <span class="red">December 1st, 2024</span>

* Paper notification: 
~~January 8th, 2025~~ <span class="red">January 10, 2025</span>

* Camera Ready Deadline:  **February 2nd, 2025**
* Workshop: <span class="red">**March 21, 2025**</span>

<div class="newsbox yellow">For your Camera Ready, please refer to the <a href="https://www.percom.org/camera-ready-preparation/">official PerCom instructions</a></div>
-->
