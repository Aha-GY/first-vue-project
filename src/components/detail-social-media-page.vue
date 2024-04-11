<template>
    <div class="page">


        <div class="part1">
            <div class="flex-iner-part1">
                <div class="flex-left"> 
                    <div id="logo">
                        <img src="@/assets/logo.png" alt="social media logo">
                    </div>
                    <div id="header">
                        <h1>Social Media Assistant</h1>
                        <p> yenigat Birhan . Addis Ababa, Ethiopia . in person</p>
                    </div>
                </div>
                <div class="flex-right">
                    <div id="apply">
                        <img src="@/assets/share.png" alt="share logo">    
                        <img src="@/assets/verticalLine.png" alt="vertical line logo">              
                        <button id="apply" @click="showButtonText('apply')"> apply</button>

                    </div>
                </div>
            </div>
        </div>


        <div class="flex-part2">

            <div class="description-right">
                <div class="description">
                    <h3> Description</h3>
                    <p> 
                        As a Social Media Assistant, you will work closely with the social media manager or marketing 
                        team to execute social media strategies and campaigns. You will be responsible 
                        for assisting in the creation and scheduling of engaging content, monitoring social media channels, and
                        interacting with followers.
                    </p>
                </div>
                <div>
                    <h3> Responsibilities</h3>
                    <ul>
                        <li>Community engagement to ensure that is supported and actively represented online</li>
                        <li>Focus on social media content development and publication</li>
                        <li>Marketing and strategy support</li>
                        <li>Stay on top of trends on social media platforms, and suggest content ideas to the team</li>
                        <li>Engage with online communities</li>
                    </ul>
                
                </div>
                <div>
                    <h3>Ideal Candidate we want</h3>
                    <ul>
                        <li>Young(18-24 year old) Female social media manager </li>
                        <li>Passionate & Reliable:  Genuine interest in our mission and a strong desire to make
                            a positive impact, responsible, and committed to fulfilling volunteer commitments.</li>
                        <li>daptable, Team Player & Strong Communication Skills: Able to work effectively in diverse teams;
                            and contributes positively.Flexible and open to embracing new challenges and shifting priorities;
                            Clear verbal and written communication, active listening, and constructive feedback. </li>
                        <li>Respectful: Embraces diversity, inclusive, and treats others with respect. Abides with all our rules 
                            and regulations </li> 
                    </ul>
                </div>
            </div>   



            <div class="about">
                <h3>about</h3>
                <ul>
                    <li>
                        <div class="flex-tags">  
                            <div><img src="@/assets/posted.png" alt=" posted logo"></div>
                            <div>
                                <p>posted on</p>
                                <p>jul 1, 2023</p>
                            </div>
                        </div>
                    </li>
                    <li>
                        <div class="flex-tags">  
                            <div><img src="@/assets/deadline.png" alt="deadline logo"></div>
                            <div>
                                <p>Deadline</p>
                                <p>jul 1, 2024</p>
                            </div>
                        </div>
                    </li>
                    <li>
                        <div class="flex-tags">  
                            <div><img src="@/assets/location.png" alt="location logo"></div>
                            <div>
                                <p>Location</p>
                                <p>Addis Ababa</p>
                            </div>
                        </div>
                    </li>
                    <li>
                        <div class="flex-tags">  
                            <div><img src="@/assets/startDate.png" alt="date logo"></div>
                            <div>
                                <p>Start Date</p>
                                <p>Aug 02, 2023</p>
                            </div>
                        </div>
                    </li>
                    <li>
                        <div class="flex-tags">  
                            <div><img src="@/assets/endDate.png" alt="date logo"></div>
                            <div>
                                <p>End Daate</p>
                                <p>sep 02, 2023</p>
                            </div>
                        </div>
                    </li>
                </ul>
                <div class="catagories">
                    <h2>Categories</h2>
                    <button id="marketing" @click="showbuttontext('Marketing')">Marketing</button>
                    <button id ="design" @click="showbuttontext('Design')">Design</button>
                </div>

                <div class="requierd">
                    <h2>Required Skills</h2>
                    <button @click="showButtonText('social media marketing')"> social media marketing </button>                    <button @click="showButtonText('English')"> English </button>
                    <button @click="showButtonText('Copywriting')"> Copywriting </button>
                </div>
            </div>
        </div>
    </div>

</template>




<style>
.part1{
    background-color: grey;
    padding: 5px;
    
}
.flex-iner-part1{
    background-color: white;
    display: flex;
    align-items: center;
    padding: 10px 15px;
    border-radius:10px ;
.flex-left{
    display: flex;
    margin-left: 10px;
}  
.flex-right{
    display: flex;
    margin-right: 10px;
}

}
.flex-part2{
    display: flex;
}

.flex-tags{
    display: flex;
}

button{
      padding : 5px 10px;
      margin-right: 10px;
      border-radius: 999px;       

}
#applay{
    background-color: blue;
}

</style>



<script>

</script>
