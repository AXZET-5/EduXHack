<template>
    <p class="Center Title Reveal">General Timeline</p>
    <div class="TimelineGrid">
        <div>
            <div class="Specialised Reveal">
                <br>
                <text class="Title">Signups&nbspopen!</text>
                <p class="Subtitle">4 May 2023</p>
                <a class="Subtitle" href="https://docs.google.com/forms/d/e/1FAIpQLSeg5M6X7YvTHgz2_iWL71TtV24U01zJvY69PMHj8paSTyrC2g/viewform" target="_blank">Start signing up here!</a>
                <br><br>
            </div>
        </div>
        <div>
            <div class="Specialised Reveal">
                <br>
                <text class="Title">Signups close</text>
                <p class="Subtitle">17 May 2023</p>
            </div>
        </div>
        <div>
            <div class="Specialised Reveal">
                <br>
                <text class="Title">Workshops</text>
                <p class="Subtitle">19 June 2023</p>
                <p class="Subtitle"></p>
            </div>
        </div>
        <div>
            <div class="Specialised Reveal">
                <br>
                <text class="Title">Hackathon!</text>
                <p class="Subtitle">20-23 June 2023</p>
                <p class="Subtitle"></p>
            </div>
        </div>
    </div>
    <div class="HorizontalLine"></div>
    <br>
    <div class="Another HorizontalLine"></div>
    <br><br>
</template>

<style scoped>
    @media only screen and (max-width: 1000px) {
        * {
        display: none;
        }
    }

    .TimelineGrid {
        display: grid;
        grid-template-columns: 1fr 1fr 1fr 1fr;
    }

    .HorizontalLine {
        background-color: #3D7DF5;
        width: 100%;
        height: 3px;
    }

    .HorizontalLine.Another {
        background-color: white;
    }

    .Specialised {
        text-align: center;
        width: 100% !important;
        background-color: rgba(0,0,0,0);
        border: none;
    }
</style>