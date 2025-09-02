Example Code (HTML + CSS to drop into your site)
<!-- Meet the Team Section -->
<section class="content-section">
  <h2 class="section-title">Meet the Team</h2>

  <div class="team-grid">
    <!-- Evan Hu -->
    <div class="team-card">
      <img src="public/images/profile-pictures/evan.webp" alt="Evan Hu" class="team-photo">
      <div class="team-info">
        <h3 class="team-name">Evan Hu</h3>
        <p class="team-role">Strategy Lead</p>
        <p class="team-desc">Evan guides our match approaches and competitive strategies.</p>
      </div>
    </div>

    <!-- Charlie Gao -->
    <div class="team-card">
      <img src="public/images/profile-pictures/charlie.webp" alt="Charlie Gao" class="team-photo">
      <div class="team-info">
        <h3 class="team-name">Charlie Gao</h3>
        <p class="team-role">Design Lead & Driver</p>
        <p class="team-desc">Charlie leads robot design and drives in competition.</p>
      </div>
    </div>

    <!-- Isabella Deng -->
    <div class="team-card">
      <img src="public/images/profile-pictures/isabella.webp" alt="Isabella Deng" class="team-photo">
      <div class="team-info">
        <h3 class="team-name">Isabella Deng</h3>
        <p class="team-role">Programming Lead</p>
        <p class="team-desc">Isabella develops our autonomous and driver-assist code.</p>
      </div>
    </div>

    <!-- Jasmine Huang -->
    <div class="team-card">
      <img src="public/images/profile-pictures/jasmine.webp" alt="Jasmine Huang" class="team-photo">
      <div class="team-info">
        <h3 class="team-name">Jasmine Huang</h3>
        <p class="team-role">Media Lead</p>
        <p class="team-desc">Jasmine manages our social media presence and team communications.</p>
      </div>
    </div>

    <!-- Ray Tan -->
    <div class="team-card">
      <img src="public/images/profile-pictures/ray.webp" alt="Ray Tan" class="team-photo">
      <div class="team-info">
        <h3 class="team-name">Ray Tan</h3>
        <p class="team-role">President</p>
        <p class="team-desc">Ray oversees the team’s vision and operations.</p>
      </div>
    </div>

    <!-- Cyrus Huang -->
    <div class="team-card">
      <img src="public/images/profile-pictures/cyrus.webp" alt="Cyrus Huang" class="team-photo">
      <div class="team-info">
        <h3 class="team-name">Cyrus Huang</h3>
        <p class="team-role">President</p>
        <p class="team-desc">Cyrus leads leadership coordination and project direction.</p>
      </div>
    </div>

    <!-- Larry Yu -->
    <div class="team-card">
      <img src="public/images/profile-pictures/larry.webp" alt="Larry Yu" class="team-photo">
      <div class="team-info">
        <h3 class="team-name">Larry Yu</h3>
        <p class="team-role">Vice President</p>
        <p class="team-desc">Larry manages logistics and supports all sub-teams.</p>
      </div>
    </div>
  </div>
</section>

CSS (add to your <style> in index.html)
/* Team Section */
.team-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 40px;
}

.team-card {
  background: var(--bright-white);
  border: 2px solid var(--light-gray);
  border-radius: 12px;
  overflow: hidden;
  box-shadow: 0 4px 12px rgba(0,0,0,0.08);
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.team-card:hover {
  transform: translateY(-4px);
  box-shadow: 0 8px 20px rgba(0,0,0,0.15);
}

.team-photo {
  width: 100%;
  height: 320px;
  object-fit: cover;
  display: block;
}

.team-info {
  padding: 20px;
  text-align: center;
}

.team-name {
  font-family: 'Etna', 'Helvetica Neue', Arial, sans-serif;
  font-size: 1.4rem;
  font-weight: 800;
  margin-bottom: 6px;
  color: var(--jet-black);
}

.team-role {
  font-size: 1.1rem;
  font-weight: 600;
  color: var(--primary-red);
  margin-bottom: 10px;
}

.team-desc {
  font-size: 0.95rem;
  color: var(--text-gray);
  line-height: 1.5;
}


✅ This will:

Respect your red/black/white branding.

Handle uneven .webp image sizes cleanly.

Recreate the card style from the screenshot but in your minimal style.

Do you want me to also make an ASCII wireframe of this section (like you asked for the site before), so you can visualize how the cards flow in grid form?