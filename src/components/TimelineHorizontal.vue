<template>
    <p class="Center Title Reveal">General Timeline</p>
    <div class="TimelineGrid">
        <div>
            <div class="Specialised Container Reveal">
                <br>
                <text class="Title">Signups&nbspopen!</text>
                <p class="Subtitle">4 May 2023</p>
                <a class="Subtitle" href="https://docs.google.com/forms/d/e/1FAIpQLSeg5M6X7YvTHgz2_iWL71TtV24U01zJvY69PMHj8paSTyrC2g/viewform" target="_blank">Start signing up here!</a>
                <br><br>
            </div>
            <div class="HorizontalLine"></div>
            <div class="Another HorizontalLine"></div>
        </div>
    </div>
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