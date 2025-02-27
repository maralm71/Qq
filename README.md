# Qq
<script>
    async function testFaceAPI() {
        try {
            await faceapi.nets.tinyFaceDetector.loadFromUri('https://cdn.jsdelivr.net/npm/face-api.js/weights/');
            await faceapi.nets.faceExpressionNet.loadFromUri('https://cdn.jsdelivr.net/npm/face-api.js/weights/');
            console.log("✅ face-api.js با موفقیت بارگذاری شد!");
        } catch (error) {
            console.error("🚨 خطا در بارگذاری face-api.js:", error);
        }
    }

    testFaceAPI();
</script>
