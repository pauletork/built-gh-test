<template>
  <div class="layout Dashboard">
    <div class="navbar-aside" id="aside-lg">
      <div class="navbar-wrapper">
        <div class="navbrand">
          <div class="navbar-logo">
            <img
              width=""
              class="logo"
              src="../assets/img/gogana-logo.svg"
              alt=""
            />
          </div>
        </div>
        <div class="menu-divider"></div>
        <div class="menu">
          <div class="menu-items">
            <div class="menu-items-wrapper">
              <div class="menu-aside-icon">
                <img width="25px" src="../assets/icons/dashboard.svg" alt="" />
              </div>
              <div class="menu-text">Dashboard</div>
            </div>
            <div class="menu-items-wrapper">
              <div class="menu-aside-icon">
                <img width="25px" src="../assets/icons/statistics.svg" alt="" />
              </div>
              <div class="menu-text">Statistics</div>
              <div class="menu-aside-pile"></div>
            </div>
            <div class="menu-items-wrapper">
              <div class="menu-aside-icon">
                <img width="15px" src="../assets/icons/payment.svg" alt="" />
              </div>
              <div class="menu-text">Payment</div>
              <div class="menu-aside-pile"></div>
            </div>
            <div class="menu-items-wrapper">
              <div class="menu-aside-icon">
                <img width="25px" src="../assets/icons/Vector.svg" alt="" />
              </div>
              <div class="menu-text">Transactions</div>
            </div>
            <div class="menu-items-wrapper">
              <div class="menu-aside-icon">
                <img width="30px" src="../assets/icons/bag.svg" alt="" />
              </div>
              <div class="menu-text">Products</div>
              <div class="menu-aside-pile"></div>
            </div>
            <div class="menu-items-wrapper">
              <div class="menu-aside-icon">
                <img width="25px" src="../assets/icons/customers.svg" alt="" />
              </div>
              <div class="menu-text">Customer</div>
              <div class="menu-aside-pile"></div>
            </div>
            <div class="menu-items-wrapper">
              <div class="menu-aside-icon">
                <img width="25px" src="../assets/icons/message.svg" alt="" />
              </div>
              <div class="menu-text">Messages</div>
              <div class="menu-aside-pile"></div>
            </div>
          </div>
          <div class="menu-bottom mb-3">
            <div class="menu-items-wrapper menu-b">
              <div class="menu-aside-icon">
                <img width="25px" src="../assets/icons/settings.svg" alt="" />
              </div>
              <div class="menu-text">Settings</div>
              <div class="menu-aside-pile"></div>
            </div>
            <div class="menu-items-wrapper">
              <div class="menu-aside-icon">
                <img width="30px" src="../assets/icons/logout.svg" alt="" />
              </div>
              <div class="menu-text">Logout</div>
              <div class="menu-aside-pile"></div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="main">
      <div class="row top-nav-wrapper">
        <div class="col-6">
          <div class="h3" id="dashboard-name">Dashboard</div>
          <div class="sm-wrapper" id="menu-sm">
            <div class="h3" id="menu-sm">
              <div class="nav-icon-wrapper">
                <div class="nav-icon-bg">
                  <img width="25" src="../assets/icons/sm-menu.svg" alt="" />
                </div>
              </div>
            </div>
            <div class="profile-section-wrapper">
              <div class="profile-section">
                <div class="search-section">
                  <div class="search-icon">
                    <img width="20px" src="../assets/icons/search.svg" alt="" />
                  </div>
                  <div class="search-placeholder text-sm">Search here...</div>
                </div>
                <div class="profile-dropdown">
                  <div class="notif-alert">
                    <img
                      width="20px"
                      style="position: abosulute; padding-left: 5px"
                      src="../assets/icons/notification.svg"
                      alt=""
                    />
                    <img
                      class="notif-indicator"
                      width="7px"
                      src="../assets/icons/dot-alert.svg"
                      alt=""
                    />
                  </div>
                </div>

                <div class="profile-avatar">
                  <img
                    width="70px"
                    class="profile"
                    src="../assets/img/paul.png"
                    alt=""
                  />
                </div>
              </div>
            </div>
          </div>
        </div>

        <div class="col-6">
          <div class="profile-section-wrapper" id="hide-profile">
            <div class="profile-section">
              <div class="search-section">
                <div class="search-icon">
                  <img width="20px" src="../assets/icons/search.svg" alt="" />
                </div>
                <div class="search-placeholder text-sm">Search here...</div>
              </div>
              <div class="profile-dropdown">
                <div class="notif-alert">
                  <img
                    width="20px"
                    style="position: abosulute; padding-left: 5px"
                    src="../assets/icons/notification.svg"
                    alt=""
                  />
                  <img
                    class="notif-indicator"
                    width="7px"
                    src="../assets/icons/dot-alert.svg"
                    alt=""
                  />
                </div>
              </div>

              <div class="profile-name">
                <h3 class="profile-name-bold">Alex Mora</h3>
                <h3 class="profile-name-light">Super Admin</h3>
              </div>

              <div class="profile-avatar">
                <img
                  width="70px"
                  class="profile"
                  src="../assets/img/paul.png"
                  alt=""
                />
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="main-divider"></div>
      <div class="row mt-4 change-mt">
        <div class="col-one-quarter">
          <div class="summary-card">
            <div class="summary-card-wrapper">
              <div class="summary-details-section mt-1">
                <div class="sales-title caption">Total Sales</div>
                <div class="sales-total h2-semi">$20.4K</div>
                <div class="sales-total text">We have sold 123 items</div>
              </div>
              <div class="summary-percentage-section">
                <apexchart
                  type="radialBar"
                  :options="chartOptions0"
                  :series="seriesD"
                >
                </apexchart>
              </div>
            </div>
          </div>
        </div>
        <div class="col-one-quarter">
          <div class="summary-card">
            <div class="summary-card-wrapper">
              <div class="summary-details-section mt-1">
                <div class="sales-title caption">Today's Revenue</div>
                <div class="sales-total h2-semi">$20.4K</div>
                <div class="sales-total text">Available to payout</div>
              </div>
              <div class="summary-percentage-section">
                <apexchart
                  type="radialBar"
                  :options="chartOptions1"
                  :series="seriesE"
                >
                </apexchart>
              </div>
            </div>
          </div>
        </div>
        <div class="col-one-quarter">
          <div class="summary-card">
            <div class="summary-card-wrapper">
              <div class="summary-details-section mt-1">
                <div class="sales-title caption">In Escrow</div>
                <div class="sales-total h2-semi">$18.2K</div>
                <div class="sales-total text">Available to payout</div>
              </div>
              <div class="summary-percentage-section">
                <apexchart
                  type="radialBar"
                  :options="chartOptions2"
                  :series="seriesF"
                >
                </apexchart>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="row mt-4 change-mt quarter-x">
        <div class="col-three-quarter">
          <div class="monthly-revenue-card">
            <div class="monthly-card-wrapper">
              <div class="chart-header">
                <div class="chart-title">
                  <div class="title caption">Total Revenue</div>
                  <div class="subtitle-box">
                    <div class="h2-semi">$50.4K</div>
                    <div class="text-sm-green ml-1" id="monthly-growth">
                      8% more than last month
                      <img width="8px" src="../assets/icons/arrow.svg" alt="" />
                    </div>
                  </div>
                </div>
                <div class="chart-options">
                  <div class="option-details text-semibold" id="update-info">
                    Data updates every 3 hours
                  </div>
                  <div class="option-action text-sm">View All Orders</div>
                </div>
              </div>
              <div class="monthly-chart">
                <div>
                  <apexchart
                    width="100%"
                    height="350px"
                    type="bar"
                    :options="optionsA"
                    :series="seriesA"
                  ></apexchart>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="col-one-quarter quarter-x">
          <div class="sales-category-card">
            <div class="category-card-wrapper">
              <div class="category-header">
                <div class="header-title caption">Most Sold Items</div>
                <div class="more-action">
                  <img
                    width="20px"
                    src="../assets/icons/icon-more.svg"
                    alt=""
                  />
                </div>
              </div>

              <div class="category-main">
                <div>
                  <apexchart
                    type="donut"
                    :options="chartOptionsDonuts"
                    :series="seriesDonuts"
                  >
                  </apexchart>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="row mt-4 change-mt">
          <div class="col-12">
            <div class="sales-table-card">
              <div class="hori-scoll">
                <div class="sales-table-wrapper">
                  <div class="table-nav">
                    <div class="table-title caption">Latest Orders</div>
                    <div class="table-details">
                      <div class="details-desc text-semibold">
                        Data updates every 3 hours
                      </div>
                      <div class="details-action text-sm-w">
                        View All Details
                      </div>
                    </div>
                  </div>
                  <div class="table-header mt-2">
                    <div class="header-product caption">Products</div>
                    <div class="header-id caption">Order ID</div>
                    <div class="header-date caption">Date</div>
                    <div class="header-customer caption">Customer name</div>
                    <div class="header-status caption">Status</div>
                    <div class="header-amount caption">Amount</div>
                    <div class="header-action caption">Action</div>
                  </div>
                  <div class="table-content">
                    <div class="header-product-content">
                      <div class="product-thumbnail-bg-1 product-thumbnail-bg">
                        <img
                          width="20px"
                          class="product-thumbnail"
                          src="../assets/icons/iphone.svg"
                          alt=""
                        />
                      </div>
                      <div class="text-semibold-b">Iphone 123 Pro</div>
                    </div>
                    <div class="header-id-content text-semibold-b">#11232</div>
                    <div class="header-date-content text-semibold-b">
                      Jun 29,2022
                    </div>
                    <div class="header-customer-content text-semibold-b">
                      Anastasis Hasuna
                    </div>
                    <div class="header-status-content text-semibold-b">
                      Delivered
                    </div>
                    <div class="header-amount-content text-semibold-b">
                      $1100.00
                    </div>
                    <div class="header-action-content text-semibold-b">
                      <img width="20px" src="../assets/icons/dots.svg" alt="" />
                    </div>
                  </div>
                  <div class="table-content">
                    <div class="header-product-content">
                      <div class="product-thumbnail-bg-2 product-thumbnail-bg">
                        <img
                          width="20px"
                          class="product-thumbnail"
                          src="../assets/icons/macbook.svg"
                          alt=""
                        />
                      </div>
                      <div class="text-semibold-b">Macbook Pro</div>
                    </div>
                    <div class="header-id-content text-semibold-b">#11233</div>
                    <div class="header-date-content text-semibold-b">
                      Jun 28,2022
                    </div>
                    <div class="header-customer-content text-semibold-b">
                      Nasuha makusta
                    </div>
                    <div class="header-status-content text-semibold-b">
                      Pending
                    </div>
                    <div class="header-amount-content text-semibold-b">
                      $1200.00
                    </div>
                    <div class="header-action-content text-semibold-b">
                      <img width="20px" src="../assets/icons/dots.svg" alt="" />
                    </div>
                  </div>
                  <div class="table-content">
                    <div class="header-product-content">
                      <div class="product-thumbnail-bg-3 product-thumbnail-bg">
                        <img
                          width="20px"
                          class="product-thumbnail"
                          src="../assets/icons/watch.svg"
                          alt=""
                        />
                      </div>
                      <div class="text-semibold-b">Apple Watch</div>
                    </div>
                    <div class="header-id-content text-semibold-b">#11234</div>
                    <div class="header-date-content text-semibold-b">
                      Jun 27,2022
                    </div>
                    <div class="header-customer-content text-semibold-b">
                      Induan Kastorika
                    </div>
                    <div class="header-status-content text-semibold-b">
                      Canceled
                    </div>
                    <div class="header-amount-content text-semibold-b">
                      $400.00
                    </div>
                    <div class="header-action-content text-semibold-b">
                      <img width="20px" src="../assets/icons/dots.svg" alt="" />
                    </div>
                  </div>
                  <div class="table-content">
                    <div class="header-product-content">
                      <div class="product-thumbnail-bg-4 product-thumbnail-bg">
                        <img
                          width="20px"
                          class="product-thumbnail"
                          src="../assets/icons/imac.svg"
                          alt=""
                        />
                      </div>
                      <div class="text-semibold-b">iMac</div>
                    </div>
                    <div class="header-id-content text-semibold-b">#11235</div>
                    <div class="header-date-content text-semibold-b">
                      Jun 26,2022
                    </div>
                    <div class="header-customer-content text-semibold-b">
                      Pogba Nehuntus
                    </div>
                    <div class="header-status-content text-semibold-b">
                      Delivered
                    </div>
                    <div class="header-amount-content text-semibold-b">
                      $200.00
                    </div>
                    <div class="header-action-content text-semibold-b">
                      <img width="20px" src="../assets/icons/dots.svg" alt="" />
                    </div>
                  </div>
                  <div class="table-content">
                    <div class="header-product-content">
                      <div class="product-thumbnail-bg-5 product-thumbnail-bg">
                        <img
                          width="20px"
                          class="product-thumbnail"
                          src="../assets/icons/ipad.svg"
                          alt=""
                        />
                      </div>
                      <div class="text-semibold-b">iPaid Air</div>
                    </div>
                    <div class="header-id-content text-semibold-b">#11236</div>
                    <div class="header-date-content text-semibold-b">
                      Jun 29,2022
                    </div>
                    <div class="header-customer-content text-semibold-b">
                      Nana Breko
                    </div>
                    <div class="header-status-content text-semibold-b">
                      Delivered
                    </div>
                    <div class="header-amount-content text-semibold-b">
                      $1700.00
                    </div>
                    <div class="header-action-content text-semibold-b">
                      <img width="20px" src="../assets/icons/dots.svg" alt="" />
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HomeView",
  components: {},
  data: function () {
    return {
      optionsA: {
        chart: {
          id: "vuechart-example",
        },
        xaxis: {
          categories: [
            "Jan",
            "Feb",
            "Mar",
            "April",
            "May",
            "Jun",
            "July",
            "Aug",
            "Sep",
          ],
        },
      },
      optionsB: {},
      optionsC: {},
      seriesA: [
        {
          name: "MRR",
          data: [30000, 40000, 45000, 50000, 49000, 60000, 70000, 91000, 45000],
        },
      ],
      seriesC: [70],
      labelsC: ["Progress"],
      seriesB: [44],

      seriesD: [75],
      seriesE: [80],
      seriesF: [60],
      chartOptions0: {
        chart: {
          height: 350,
          type: "radialBar",
        },
        plotOptions: {
          radialBar: {
            hollow: {
              size: "75%",
            },
          },
        },
        labels: ["Progress"],
      },
      chartOptions1: {
        chart: {
          height: 350,
          type: "radialBar",
        },
        plotOptions: {
          radialBar: {
            hollow: {
              size: "80%",
            },
          },
        },
        labels: ["Progress"],
      },
      chartOptions2: {
        chart: {
          height: 350,
          type: "radialBar",
        },
        plotOptions: {
          radialBar: {
            hollow: {
              size: "60%",
            },
          },
        },
        labels: ["Progress"],
      },
      seriesDO: [44, 55, 41, 17, 15],
      chartOptionsDO: {
        labelsDO: ["Apple", "Mango", "Orange", "Watermelon"],
        customScale: 0.8,
        pie: {
          size: 200,
          donut: {
            size: "65%",
          },
        },
      },
      seriesDonuts: [25, 25, 25, 25],
      chartOptionsDonuts: {
        labels: ["Jeans", "Shirts", "Caps", "Others"],
        chart: {
          type: "donut",
        },
        responsive: [
          {
            breakpoint: 480,
            options: {
              chart: {
                width: "100%",
              },
              legend: {
                position: "bottom",
              },
            },
          },
        ],
      },
      seriesBar: [
        {
          data: [400, 430, 448, 470, 540, 580, 690, 1100, 1200, 1380],
        },
      ],
      chartOptionBar: {
        chart: {
          type: "bar",
          height: 350,
        },
        plotOptions: {
          bar: {
            borderRadius: 4,
            horizontal: false,
            vertical: true,
          },
        },
        dataLabels: {
          enabled: false,
        },
        xaxis: {
          categories: [
            "South Korea",
            "Canada",
            "United Kingdom",
            "Netherlands",
            "Italy",
            "France",
            "Japan",
            "United States",
            "China",
            "Germany",
          ],
        },
      },
    };
  },
};
</script>
