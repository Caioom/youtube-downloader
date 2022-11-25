<script>
  import Header from './Header.svelte'
</script>
<style>
  .alignAsColumn {
    flex-direction: column;
  }

  .centerDisplayFlex {
    display: flex;
    align-self: center;
    justify-content: center;
  }

  .container {
    height: 100vh;
    width: 25%; 
  }

  #uploadFileInput {
    display: none;
  }

  .uploadFileLabel {
    cursor: pointer;
    border: solid 1px #000;
    width: 100%;
    height: 25%;
  }

  .downloadButton {
    margin-top: 5px;
  }

</style>
<Header />
<div class="container centerDisplayFlex alignAsColumn">
  <p>Insert here your file here:</p>
  <label for="uploadFileInput" class="uploadFileLabel centerDisplayFlex">
    <input id="uploadFileInput" type="file"/>
  </label>
  <button class="downloadButton">Download</button>
</div>