<template>
  <!-- this is an object to describe one view on the page -->
  <main class="content-area">
    <div class="content-bubble">
      <h2 class="content-title">
        Article Title
      </h2>
      <div class="content-bubble-text-area">
        <p>
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse eu imperdiet massa. Phasellus dictum eros euismod mi gravida tristique. Vivamus hendrerit porta metus in rhoncus. Aliquam tempor a nibh ut tincidunt. Etiam maximus ligula et massa faucibus, et auctor dolor dictum. Curabitur ut imperdiet eros, fermentum aliquet felis. Cras pharetra non diam sed finibus. Nunc nulla augue, dictum sit amet ante et, luctus pellentesque risus.
        </p>
        <p>
    Curabitur efficitur tortor augue, non pellentesque lorem pretium at. Mauris euismod massa nisl, mollis tincidunt orci commodo fermentum. Vestibulum porttitor dui vel nunc blandit luctus. In mattis ipsum eget sapien dictum malesuada. Praesent porttitor fermentum augue nec consequat. Phasellus maximus ex a eros mattis gravida. Suspendisse id ligula ullamcorper, volutpat urna consectetur, hendrerit diam. Fusce enim eros, sagittis non ante eu, dapibus laoreet nulla. Nunc lorem nunc, feugiat in aliquet quis, porta vitae nunc. Nullam vehicula sem vestibulum, scelerisque magna id, volutpat dolor. Duis tempor nisi in ex vulputate dictum. Quisque sagittis ultrices odio rhoncus pharetra. Integer ut lacus finibus dolor fringilla interdum. Nulla facilisi.
        </p>
        <p>
    Vivamus nec enim at libero pretium suscipit. Praesent ut venenatis sapien. Sed sed diam odio. Curabitur euismod varius massa non porttitor. Integer eu lectus ipsum. Nam in dolor metus. Pellentesque vitae odio convallis, fermentum libero sed, sodales erat. Nulla facilisi. Suspendisse potenti. Aliquam erat volutpat. Proin consectetur nisi sed metus bibendum molestie vel id mauris. Cras sit amet lobortis lorem.
        </p>
        <p>
    Sed in ligula non arcu sodales finibus ac nec purus. Integer dapibus lectus id neque malesuada, vitae consequat dolor tincidunt. Ut pulvinar est accumsan libero auctor, et venenatis neque blandit. Nunc venenatis nulla sagittis ultrices sagittis. Donec a imperdiet dui, eget ullamcorper urna. Aliquam ultricies nunc felis, vel consectetur velit consectetur ut. Vivamus feugiat tincidunt ultrices. Vivamus varius elit arcu, in porta dui blandit eget. In elementum eu lorem eget auctor.
        </p>
        <p>
    Cras condimentum, ligula ac lobortis volutpat, mauris nisi viverra augue, vel laoreet nulla dolor sit amet felis. Phasellus elementum, mi nec luctus hendrerit, justo diam auctor est, et suscipit orci lorem quis quam. Mauris elementum sed magna quis faucibus. Aenean feugiat lobortis mattis. Quisque vestibulum eu dui sit amet vulputate. Donec sem quam, ultricies eu feugiat et, consectetur et diam. Etiam in egestas risus. Donec et dolor diam. Nullam eu libero egestas, viverra diam ac, maximus enim. Morbi bibendum massa rutrum felis rhoncus dapibus. Praesent vel vulputate mi, a vehicula lectus. Nunc gravida, dolor vel pulvinar ultrices, diam elit fermentum dolor, vitae ultrices nibh nibh et justo. Vivamus eleifend feugiat magna, ut dapibus dui tempor vitae. In posuere, sapien ac laoreet suscipit, tellus velit venenatis felis, nec imperdiet elit diam ac quam. Fusce consequat ipsum eget leo rutrum, et efficitur ex tincidunt. Nam tellus lorem, imperdiet nec tincidunt vitae, egestas a eros. 
        </p>
      </div>
    </div>
    <div class="f3-button-tray">
      <button class="btn btn-light f3-button">I</button>
      <button class="btn btn-light f3-button">II</button>
      <button class="btn btn-light f3-button">III</button>
    </div>
  </main>
</template>

<script>
export default {
  name: "TextView",
};
</script>

<style>
  #TextView{
    display:flex;
  }
  .content-area {
    display: flex;
    flex-direction: row;
    justify-content: center;    /* not working on h2 */
    align-content: center;
  }
  .content-bubble {
    padding: 2em 1em;
    margin: 1em;
    max-width: 720px;
    max-height: 800px;
  }

  .content-bubble>*{
    background-color: #2c3e50e8;
    padding: 1em;
  }

  .content-bubble-text-area {
    max-width:720px;
    max-height:600px;
    overflow-y:auto;    /* overflow only works for specified height */
    margin-bottom: 5px;
  }

  .content-title {
    width: fit-content;
    padding: 1em 1em;
    margin: auto auto 1em auto;
    justify-self: center;
  }

  /* button area */
  .f3-button-tray { /* need to add viewport option - if on phone, these buttons go to top of the container and the container itself shifts to flex-column*/
    display: flex;
    flex-direction: column;
    justify-content: center;
  }

  .f3-button {
    margin-bottom: 5px;
  }

</style>