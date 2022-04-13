<script>
export default { }
</script>

<template>
    <div class="p-4 p-md-5 mb-4 rounded bg-light">
        <div class="row align-items-center">
            <h1 class="display-6">
                Would you like to see more tips and tutorials on web
                development ?
            </h1>

            <form class="row g-3">
                <div class="col-md-6">
                    <label for="inputFirstName" class="form-label">First Name</label>
                    <input type="text" class="form-control" id="inputFirstName" />
                </div>
                <div class="col-md-6">
                    <label for="inputLastName" class="form-label">Last Name</label>
                    <input type="text" class="form-control" id="inputLastName" />
                </div>
                <div class="col-12">
                    <label for="inputEmail" class="form-label">Email</label>
                    <input type="email" class="form-control" id="inputEmail" />
                </div>
                <div class="col-12">
                    <button type="submit" class="btn btn-primary">Subscribe</button>
                </div>
            </form>
        </div>
    </div>
</template>