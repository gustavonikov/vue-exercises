.<template>
    <div class="gift-container">
        <div class="tie">
            <div class="left-tie"></div>
            <div class="right-tie"></div>
        </div>
        <div class="gift">
            <div class="gift-tie-1"></div>
            <div class="gift-tie-2"></div>
            <div class="gift-top"></div>
            <div class="gift-body"></div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Gift',
};
</script>

<style>
    .tie {
        display: flex;
        align-items: center;
        justify-content: center;

        margin-bottom: -1px;
    }

    .left-tie {
        width: 45px;
        height: 30px;
        border: 8px solid #f00;
        border-top-width: 10px;
        border-left-width: 10px;
        border-top-left-radius: 25px;
        border-top-right-radius: 25px;
        border-bottom-left-radius: 20px;
        border-bottom-right-radius: 20px;

        transform: skewY(18deg);

        margin-right: -2px;

        filter: brightness(0.98);

        z-index: 30;
    }

    .right-tie {
        width: 45px;
        height: 30px;
        border: 8px solid #f00;
        border-top-width: 10px;
        border-left-width: 10px;
        border-top-left-radius: 25px;
        border-top-right-radius: 25px;
        border-bottom-left-radius: 20px;
        border-bottom-right-radius: 20px;

        transform: skewY(-18deg) rotateY(180deg);

        filter: brightness(0.98);
        
        z-index: 30;
    }

    .gift {
        position: relative;
        display: flex;
        flex-direction: column;
        align-items: center;
        z-index: 10;
    }

    .gift-top {
        width: 100px;
        height: 25px;
        background-color: #7aa944;
    }

    .gift-body {
        width: 90px;
        height: 60px;
        background-color: #5c7e32;
    }

    .gift-tie-1 {
        position: absolute;
        width: 15px;
        height: 85px;
        background-color: #f00;
    }

    .gift-tie-2 {
        position: absolute;
        top: 40px;
        width: 90px;
        height: 15px;
        background-color: #f00;
    }
</style>