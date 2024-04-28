<script>
async function fetchData(url) {
    try {
        const response = await fetch(url);
        if (!response.ok) {
            throw new Error(`API request failed with status ${response.status}`);
        }
        const data = await response.json();
        return data;
    } catch (error) {
        console.error('Error fetching data:', error);
        return { message: 'API currently unavailable' }; // Handle error by returning a custom message
    }
}

async function populateCards() {
    const data = await fetchData('https://akil-backend.onrender.com/');
    const cardsContainer = document.getElementById('cards-container');

    cardsContainer.innerHTML = '';

    const messageElement = document.createElement('p');
    messageElement.textContent = data.message;
    cardsContainer.appendChild(messageElement);
}

</script>