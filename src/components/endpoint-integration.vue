<script>
    // Assuming some sample opportunity data structure
const mockData = [
    { title: 'Software Engineer Internship', description: 'Develop and test innovative software solutions...' },
    { title: 'Volunteer at Animal Shelter', description: 'Care for animals and assist with shelter operations...' },
    // ... more mock opportunities
];

async function populateCards() {
    // No need for fetchData in this case (using mock data)

    const cardsContainer = document.getElementById('cards-container');
    cardsContainer.innerHTML = '';

    mockData.forEach(opportunity => {
        const card = createCardElement(opportunity);
        cardsContainer.appendChild(card);
    });
}

function createCardElement(opportunity) {
    // ... same logic as before to create card elements from data
}

</script>