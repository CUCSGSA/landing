---
layout: page
---

<style>
.event {
    display: flex;
    flex-direction: column; /* Align children (title, image+text) in a column */
    margin-bottom: 20px; /* Adds space between events */
}

.event h3 {
    margin-bottom: 10px; /* Space between title and image+text container */
}

.event > div {
    display: flex;
    align-items: center;
    width: 100%;
}

.event img {
    width: 30%; /* Adjust image width as necessary */
    margin-right: 20px;
}

.event div {
    width: 70%; /* Adjust text container width */
}
</style>

# GPDC and CSGSA Events Page

Welcome to our collaborative events page! Here, you will find detailed information about the activities and events organized by both the Graduate Professional Development Club (GPDC) and the Computer Science Graduate Student Association (CSGSA). Our offerings range from professional development workshops to cultural festivities, all designed to enrich your university experience.



<button onclick="filterEvents('GPDC')">GPDC</button>
<button onclick="filterEvents('CSGSA')">CSGSA</button>
<button onclick="filterEvents('all')">All</button>


# September 2024

<div class="event" data-club="GPDC">
    <h2>Industry Speaker Series</h2>
    <div style="display: flex; align-items: center;">
        <img src="assets/img/speaker_series.jpg" alt="September Speaker Series" style="width: 50%; margin-right: 20px;">
        <div>
            <p>Join us for enlightening discussions with industry experts about the evolving landscape of technology and business. These sessions provide insights into emerging industry trends and professional development opportunities. </p> 
            
            <h3>When? September 13th </h3>
            <h3> Where? DLC1B70 </h3>
        </div>
    </div>
</div>

# October 2024

<div class="event" data-club="CSGSA">
    <h2>Cross Cultural Celebrations </h2>
    <div style="display: flex; align-items: center;">
        <img src="assets/img/cross_cultural_celebration.jpg" alt="Cross Cultural Celebrations" style="width: 50%; margin-right: 20px;">
        <div>
            <p>Celebrate the rich diversity of our community with a potluck, featuring dance and musical performances. A vibrant display of cultures, this event is a cornerstone of our fall semester activities.</p>
            <h3>When?  October 11th</h3>
            <h3> Where?  DLC 1B70</h3>
        </div>
    </div>
</div>

<div class="event" data-club="GPDC">
    <h2>Industry Speaker Series </h2>
    <div style="display: flex; align-items: center;">
        <img src="assets/img/speaker_series.jpg" alt="October Speaker Series" style="width: 50%; margin-right: 20px;">
        <div>
            <p>Continue your professional growth with another talk by an expert who will delve into the nuances of technological advancements and career development.</p>
            <h3>When?  October 18th</h3>
            <h3> Where? tbd </h3>
        </div>
    </div>
</div>

<div class="event" data-club="GPDC">
    <h2>Mock Interviews</h2>
    <div style="display: flex; align-items: center;">
        <img src="assets/img/mock_interviews.jpg" alt="Mock Interviews" style="width: 50%; margin-right: 20px;">
        <div>
            <p>Gain practical experience and personalized feedback from industry professionals to prepare for real job interviews. This event is a must for those seeking internships or full-time positions.</p>
            <h3>When?  October 25th</h3>
            <h3> Where?  Kitteredge Central</h3>
        </div>
    </div>
</div>

# November 2024

<div class="event" data-club="GPDC">
    <h3>Industry Speaker Series</h3>
    <div style="display: flex; align-items: center;">
        <img src="assets/img/speaker_series.jpg" alt="November Speaker Series" style="width: 50%; margin-right: 20px;">
        <div>
            <p>Our final speaker event of the semester offers a unique opportunity to engage with experts in the industry and discover career paths you might never have considered.</p>
            <h3>When? November 8th </h3>
            <h3> Where? tbd </h3>
        </div>
    </div>
</div>

<div class="event" data-club="GPDC">
    <h2>Code Buffer </h2>
    <div style="display: flex; align-items: center;">
        <img src="assets/img/fall_coding_challenge.jpg" alt="Fall Coding Challenge" style="width: 50%; margin-right: 20px;">
        <div>
            <p>Compete in our prestigious coding challenge for a chance to win substantial cash prizes and demonstrate your coding expertise in a competitive yet friendly environment.</p>
            <h3>When?  November 15th</h3>
            <h3> Where? DLC1B70 </h3>
        </div>
    </div>
</div>

<div class="event" data-club="CSGSA">
    <h2>Friendsgiving</h2>
    <div style="display: flex; align-items: center;">
        <img src="assets/img/friendsgiving.jpg" alt="Friendsgiving" style="width: 50%; margin-right: 20px;">
        <div>
            <p>Join us for a heartwarming celebration of thanks and gratitude as we gather together to share a meal and give back to the community through our food drive.</p>
            <h3>When? November 21st </h3>
            <h3> Where? DLC1B70 </h3>
        </div>
    </div>
</div>

<div class="event" data-club="CSGSA">
    <h2>Town Hall Meeting</h2>
    <div style="display: flex; align-items: center;">
        <img src="assets/img/town_hall.jpg" alt="Town Hall Meeting" style="width: 50%; margin-right: 20px;">
        <div>
            <p>Discuss vital departmental issues, such as student facilities and other important topics, in this forum. Your input directly influences our ability to advocate for improvements within the department.</p>
            <h3>When?  November 21st</h3>
            <h3> Where? DLC1B70 </h3>
        </div>
    </div>
</div>

# December 2024

<div class="event" data-club="CSGSA">
    <h2>TeaTime++</h2>
    <div style="display: flex; align-items: center;">
        <img src="assets/img/tea_time.jpg" alt="TeaTime++" style="width: 50%; margin-right: 20px;">
        <div>
            <p>Enjoy an extended version of our regular Tea Time, with more snacks, a variety of teas, and plenty of time for those longer board games that are perfect for strategic thinkers.</p>
            <h3>When? December 8th </h3>
            <h3> Where? DLC1B70 </h3>
        </div>
    </div>
</div>

<script>
function filterEvents(club) {
    const events = document.querySelectorAll('.event');
    events.forEach(event => {
        if (event.getAttribute('data-club') === club || club === 'all') {
            event.style.display = 'flex';
        } else {
            event.style.display = 'none';
        }
    });
}
</script>
